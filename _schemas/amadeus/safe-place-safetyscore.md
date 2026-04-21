---
description: ''
layout: schema
name: SafetyScore
properties_list:
- description: Likelihood of inappropriate behavior against females. Score go from 1 (not likely) to 100 (very likely).
  name: women
  type: integer
- description: Likelihood of injury due to harmful intent. Score go from 1 (not likely) to 100 (very likely).
  name: physicalHarm
  type: integer
- description: Likelihood of theft. Score go from 1 (not likely) to 100 (very likely).
  name: theft
  type: integer
- description: Potential for infringement of political rights or political unrest. Score go from 1 (not likely) to 100 (very likely).
  name: politicalFreedom
  type: integer
- description: Likelihood of harm or discrimination against LGBTQ persons or groups and level of caution required at location. Score go from 1 (not likely) to 100 (very likely).
  name: lgbtq
  type: integer
- description: Likelihood of illness or disease, assessment of water and air quality, and access to reliable medical care. Score go from 1 (not likely) to 100 (very likely).
  name: medical
  type: integer
- description: An average of the 6 “sub”-categories. Score go from 1 (very safe) to 100 (very dangerous).
  name: overall
  type: integer
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/safe-place-safetyscore-schema.json
slug: safe-place-safetyscore
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: SafetyScore
---
