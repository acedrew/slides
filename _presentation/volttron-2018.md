---
layout: slideshow
theme: ace-iot

author: "Andrew Rodgers"
title:  "Eclipse VOLTTRON&trade; DC Deployment Updates"
company: "Ace IoT Solutions"
email: info@aceiotsolutions.com
website: aceiotsolutions.com
twitter: acedrew
instagram: acedrewcha

slides:
  - format: intro
    notes: Don't forget this is an intro
    footer: hidden

  - format: sectionbreak
    title: ! "intro: Who we are"

  - format: sectionbreak
    title: ! "ACE IoT Solutions"

  - format: single
    text: Supporting the DC DGS deployment of VOLTTRON&trade; since late 2016

  - format: single
    text: Focused on developing tools and providing services to companies wanting to operationalize VOLTTRON&trade;
    notes: Call us for that support Eclipse won't give you

  - format: sectionbreak
    title: ! "intro: Where we've been"

  - format: single
    text: VOLTTRON&trade; 2017

  - format: single
    text: <10 sites

  - format: list
    title: "What we had:"
    list:
      - implemented basic deployment system
      - implemented centralized logging system
      - implemented infrastructure monitoring system
      - implemented data discovery layer using open source dashboarding tools
      - integrated with existing dashboarding and analytics software in the enterprise
    footer: hidden

  - format: list
    title: "Pain points:"
    list:
      - still required command line competency for deployment of new sites
      - config management was completely manual, no centralized config for drivers
      - 3rd party tools used for site data discovery
    footer: hidden

  - format: sectionbreak
    title: "What We've done:"

  - format: sectionbreak
    title: Deployment

  - format: list-step
    title: Basic Deployment for our use-case
    list:
      - text: Install hardware on site
      - text: |
          Initiate <br>
          BACnet Scan
      - text: Generate device and registry configs
    footer: hidden

  - format: single
    text: Rinse and Repeat as necessary

  - format: single
    text: Profit?

  - format: single
    text: Slow (painful) command line deployment process
    notes: each of these steps represented a command line competent person

  - format: sectionbreak
    title: "Deployment now:"

  - format: list-step
    slide-transition: "slide-in fade-out"
    title: Basic Deployment for our use-case
    list:
      - text: Install hardware on site
        selected: true
      - text: |
          Initiate <br>
          BACnet Scan
      - text: Generate device and registry configs
    footer: hidden

  - format: single
    text: Equipment OEM loads base image on our devices
    notes: Reference terry

  - format: single
    text: Simple interface for most common deployment tasks

  - format: image
    image: '/volttron-2018/deploy-screen-main.png'
    footer: hidden

  - format: single
    text: Deploying a new site

  - format: image
    image: '/volttron-2018/deploy-screen-new.png'
    footer: hidden
    notes: replacing static ip with dynamic queue

  - format: list-step
    slide-transition: "slide-in fade-out"
    title: Basic Deployment for our use-case
    list:
      - text: Install hardware on site
      - text: |
          Initiate <br>
          BACnet Scan
        selected: true
      - text: Generate device and registry configs
    footer: hidden

  - format: single
    text: "Scan BACnet for a site:"

  - format: image
    image: '/volttron-2018/deploy-screen-bacnet-scan.png'
    footer: hidden
    notes: replacing static ip with dynamic queue

  - format: single
    text: Filter and tag using separate tools 

  - format: list-step
    slide-transition: "slide-in fade-out"
    title: Basic Deployment for our use-case
    list:
      - text: Install hardware on site
      - text: |
          Initiate <br>
          BACnet Scan
      - text: Generate device <br> and registry configs
        selected: true
    footer: hidden

  - format: single
    text: Generate configs

  - format: image
    image: '/volttron-2018/deploy-screen-config-deploy.png'
    footer: hidden
    notes: all device and registry configs built and installed automatically

  - format: single
    text: Repeat ad infinitum 

  - format: single
    text: Additional tool for testing new feature and releases

  - format: image
    image: '/volttron-2018/deploy-screen-redeploy.png'
    footer: hidden
    notes: all device and registry configs built and installed automatically

  - format: single
    text: Deterministic test suites?

  - format: thanks
    title: Thank You
    footer: hidden

  - format: contact
    footer: hidden

---
