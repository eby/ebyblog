+++
date = '2026-09-18T13:39:25-04:00'
title = 'Polycom Phones and UniFi'
+++
We recently migrated to new Polycom phones. Our old ones were set for a specific vlan in provisioning, but this batch we had more default settings so we could different VLANs at different sites.

At sites with Juniper switches the LLDP worked great and all the phones got their new VLANs. At UniFi sites some phones would work, some would get stuck on the native VLAN and some would get stuck in a reboot loop, hopping between them. On the gateway we had a port profile for the phones with LLDP enabled and voice vlan set.

### UniFi timing bug

After searching the forums, I was able to find multiple people in the same boat: [Ubiquiti Community thread about LLDP-MED and Polycom phones](https://community.ui.com/questions/LLDP-MED-for-VOIP-phones-issue-Thoughts-and-help/09560696-9ec3-4b6d-a76c-94fcafdb6b5a). 

One workaround is to SSH to each switch and change the LLDP interval from the default 30 seconds to five seconds:

```text
telnet 127.0.0.1
enable
configure
lldp timers interval 5
```

That change makes voice-VLAN advertisements arrive often enough for the phones to stay where they belong. It is lost on reboots and provisioning, though.  

Other reference:

- [UniFi thread about the LLDP interval timer and Polycom phones](https://community.ui.com/questions/LLDP-MED-Interval-timer-issue-with-PolyCom-Phones-and-Voice-VLAN/2693e24a-6361-4d54-8ffd-54c781414e6f) 
- [Polycom phones and Ubiquiti switches](https://hochwald.net/polycom-ip-phones-and-ubiquiti-switches/) 

### DHCP Workaround

The most reliable route, from what I can tell, is to disable LLDP on the Unifi ports and go with other methods like DHCP. If LLDP is enabled then the phones will ignore the DHCP options.

The Polycom models we got, with default settings, have VLAN blank and DHCP discovery set to fixed. 

This means it checks DHCP options 128, 144, 157 and 191 in order until it finds a valid string.

For UniFi you would add this as a custom DHCP option. For ISC DHCP it would look something like this:

```text
option polycom_vlan code 144 = text;
option polycom_vlan "VLAN-A=7;";
```

The code definition can be global and the VLAN-A option would be on any of the native VLANs a phone might be hooked to. In this example 7 is the voice VLAN.

Source: [[FAQ] Utilizing VLAN's with Polycom phones](https://h30434.www3.hp.com/t5/Poly-Phones-Knowledge-Base/FAQ-Utilizing-VLAN-s-with-Polycom-phones/ta-p/9605324)

### Other Useful DHCP Options

These all go on the Voice VLAN

- 42 (NTP) The NTP server in IP format. Usually provided by the phone provider
- 66 (TFTP) The provisioning server without the protocol like `provisioning.example.com`
- 160 The provisioning server URL with the protocol like `http://provisioning.example.com`
