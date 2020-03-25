---
title: Host Identity Protocol
layout: slideshow
theme: personal
author: Andrew Rodgers
email: acedrew@gmail.com
website: aceiotsolutions.com
twitter: acedrew
instagram: acedrewcha
slides:
- format: intro
  notes: Don't forget this is an intro
  footer: hidden
- format: sectionbreak
  title: "Hi, I'm Andrew"
- format: single
  title: "and I don't buy bullshit"
  text: " "
- format: sectionbreak
  title: 'why am I here?'
- format: single
  text: to give a talk about Host Identity Protocol (HIP)
- format: single
  text: actually to rant about technology marketing
- format: single
  text: "we'll get to the paper..."
- format: single
  text: "this talk is brought to you by a salesperson's empty promises"
- format: single
  text: 'About a year ago, someone said'
- format: sectionbreak
  title: 'have you heard of HIP?'
- format: image
  image: "/hip-talk/schitts-creek-honest.gif"
  background-size: contain
  footer: hidden
- format: single
  text: "I fucked up - Tim Berners-Lee"
- format: image
  image: "/hip-talk/invisibility-is-security.png"
  background-size: contain
  footer: hidden
- format: single
  text: "but I digress"
- format: single
  text: "What is HIP?"
- format: single
  text: "RFC 5201"
- format: single
  text: "Work started in the late 90s, RFC was published in 2008"
- format: single
  text: "We're focusing on an overview paper published by Nikander, Gurtov and Henderson in 2009"
- format: single
  text: "Audacious goal, compeletely replace IP and DNS while integrating IPv6"
- format: single
  text: "For those of you that believe in OSI Layers"
- format: image
  image: "/hip-talk/hip-layers.png"
  background-size: contain
  footer: hidden
- format: list
  title: 'Core Goals'
  list:
  - Non-Mutabilty
  - Location Independence
  - Reversibility
  - Omnisciency
  footer: hidden
- format: single-topbar
  title: "Non-Mutability"
  text: "The source and destination identities sent are the identities received."
- format: single-topbar
  title: "Location Independence"
  text: "The identities do not change during the course of an ”association”."
- format: single-topbar
  title: "Reversibility"
  text: "A return header can always be formed by reversing the source and destination identities."
- format: single-topbar
  title: "Omnisciency"
  text: "Each host knows what identities a peer host can use to send packets to it."
- format: single
  text: "theoretical beauty"
- format: single
  text: "All host/service identifiers are replaced with cryptographically verifiable hashes"
- format: single
  text: "All communications, including control packets are encrypted"
- format: single
  text: "Perfect for IPv6, uses a specific prefix, then a 100 bit hash of the host key as the address"
- format: single
  text: "These 128 bit Host Identity Tags (HIT) are considered cryptographically verifiable to be from the Host Identities associated"
- format: single
  text: separates addressing from locating for communications
- format: image
  image: "/hip-talk/hip-exchange.png"
  background-size: contain
  footer: hidden
- format: sectionbreak
  title: "in reality:"
- format: single
  text: "Brand new protocol"
- format: single
  text: "Brand new namespace"
- format: single
  text: "A preliminary study concluded that a name resolution system that scales up to millions of mobile hosts can be constructed for HIP"
- format: single
  text: "Needs support in all underlying network infrastructure"
- format: single
  text: "But wait, it's backwards compatible, how?"
- format: single
  text: "It's encapsulatable in UDP using the same techniques that IPSEC is currently transported"
- format: single
  text: "what this means in applications:"
- format: image
  image: "/hip-talk/hip-talk-ace-network.png"
  background-size: contain
  footer: hidden
- format: image
  image: "/hip-talk/hip-talk-ace-network-hip.png"
  background-size: contain
  footer: hidden
- format: single
  text: "It's a VPN"
- format: single
  text: "Use WireGuard"
- format: thanks
  title: Thank You
  footer: hidden
- format: contact
  footer: hidden
---

