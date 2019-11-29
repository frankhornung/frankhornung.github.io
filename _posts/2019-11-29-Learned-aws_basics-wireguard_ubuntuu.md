---
layout: post
title: learning about AWS and VPN technologies (wiregurad/openvpn/mullvad) 
tags: [wireguard, aws, mullvad, openvpn]
---

# AWS introduction webinar attended
Today i had the chance to participate in a AWS introduction webinar at work.
* AWS introduction
* EC2 instances, spot instances, reserved instances
* storage: EBS, S3...
* networking: VPC, CloudFront, ELB


# Mullvad VPN on Ubuntu 19.04
i want to use my mullvad vpn account on my notebook when travelling (e.g. on a public train)
## setting up Wireguard with Mulvad on Ubuntu 19.04
The first option is to setup native wireguard connection using the commandline

* set up APT package source
* install wireguard dkms
* uefi secure boot MOK management
* wg-quick tool fails - does not work for me out of the box

[ubuntuusers wiki on wireguard](https://wiki.ubuntuusers.de/WireGuard/)
[mullvad linux setup guide](https://mullvad.net/de/help/easy-wireguard-mullvad-setup-linux/)

## setting up Mullvad App (OpenVPN)
the second option is to use the nice mullvad app that uses OpenVPN as a VPN technology behind the scenes.
I used this guide to set it up
[mullvad app on linux](https://mullvad.net/de/help/install-mullvad-app-linux/)

some screenshots:

the nice desktop app itself
![mullvad_vpn_app.png](/images/mullvad_vpn_app.png)


this is shown in your notification bar (gnome)
![mullvad_vpn_icon.png](/images/mullvad_vpn_icon.png)
