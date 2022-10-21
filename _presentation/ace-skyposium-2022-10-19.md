---
title: "ACE Skyspark: Streaming data into Skyspark from conventional data pipelines"
layout: slideshow
theme: ace-iot
author: Andrew Rodgers
company: Ace IoT Solutions
email: andrew@aceiotsolutions.com
website: aceiotsolutions.com
twitter: acedrew
venue: SkyPosium 2022
slides:
- format: intro
  notes: Don't forget this is an intro
  footer: hidden
- format: sectionbreak
  title: ACE IoT Solutions
- format: single
  text: Software Company founded in 2018 based in Chattanooga, Tennesee
- format: single
  text: ACE IoT Solutions leverages open source technologies, including the Eclipse
    VOLTTRON™ platform
- format: single
  text: We provide our customers with low cost approaches to securely acquire, access
    and manage data from distributed control systems and sensors.
- format: sectionbreak
  title: ACE's approach to data acquisition
- format: image
  image: "/ace-skyposium-2022-10-19/ace-network-diagram.svg"
  footer: hidden
  background-size: auto 90%
  background-color: "#fff"
  background-transition: slide
- format: image
  image: "/ace-skyposium-2022-10-19/ace-network-diagram-skyspark.svg"
  footer: hidden
  background-size: auto 90%
  background-color: "#fff"
  background-transition: slide
- format: sectionbreak
  title: "Approaches"
- format: list-step
  title: 'Existing options:'
  list:
  - text: Implement API adaptor in Skyspark
  - text: PySession/hxpy
  - text: PyHaystack
  footer: hidden
- format: list-step
  title: 'Existing options:'
  list:
    - text: Implement API connector in Skyspark
      selected: true
    - text: PySession/hxpy
    - text: PyHaystack
  footer: hidden
- format: list
  title: Native API connector
  list:
    - None of us are Fantom or Axon devs
    - Would need to install and maintain in all customer environments
    - Backfilling and troubleshooting would have to be managed from client environments
    - Likely miss out on our evented architecture, resulting in higher API load
  footer: hidden
- format: list-step
  title: 'Existing options:'
  list:
    - text: Implement API adaptor in Skyspark
    - text: PySession/hxpy
      selected: true
    - text: PyHaystack
  footer: hidden
- format: list
  title: PySession/hxpy
  list:
    - Requires SkySpark to manage containers, not compatible with AWS Lambda or other FaaS infrastructure
    - If using pull, would need to deploy and manage container environments in customer sites
    - Not really the use case it was designed for, likely to encounter support issues
    - We really try to be open-first, customers should have choice, even if the best choice is SkySpark
  footer: hidden
- format: list-step
  title: 'Existing options:'
  list:
    - text: Implement API adaptor in Skyspark
    - text: PySession/hxpy
    - text: PyHaystack
      selected: true
  footer: hidden
- format: list
  title: PyHaystack
  list:
    - Open Source! (by great people, shout-out Christian)
    - Standard Python runtime allows us to run anywhere Python is supported
    - Oriented around syncing metadata and bulk data import/export, not ideal for streaming
    - Broader use-case, meant to support multiple vendor's Haystack APIs, with various auth options
    - Initial implementation for a relatively small site resulted in 100s of API calls to SkySpark for each time-step
  footer: hidden
- format: list-step
  title: 'Options:'
  list:
    - text: Implement API adaptor in Skyspark
    - text: PySession/hxpy
    - text: PyHaystack
    - text: ace-skyspark
      selected: true
  footer: hidden
- format: list
  title: "ace-skyspark:"
  list:
    - Open Source! (by ok people, shout-out us)
    - Standard Python runtime allows us to run anywhere Python is supported
    - Oriented around efficiently streaming time series data into SkySpark
    - Single purpose, meant to be useful to the SkySpark community without complexity of supporting broader ecosystem
    - Not intended as a monolith, composable architecture allows using the pieces you need and ignoring the rest
  footer: hidden
- format: sectionbreak
  title: Demo Time 🤐
- format: list
  title: "ace-skyspark future:"
  list:
    - Open Source! (contribute if you want) https://github.com/ACE-IoT-Solutions/ace-skyspark
    - Support more metadata synchronization options
    - Use Haxall/hxpy models
    - Include more direct support for Pandas/Numpy data structures
    - Open to better ways...
  footer: hidden
- format: sectionbreak
  title: Questions?
- format: thanks
  title: Thank You
  footer: hidden
- format: contact
  footer: hidden
---

