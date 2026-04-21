---
description: Restriction towards carriers.
layout: schema
name: CarrierRestrictions
properties_list:
- description: 'This flag enable/disable filtering of blacklisted airline by EU. The list of the banned airlines is published in the Official Journal of the European Union, where they are included as annexes A and B '
  name: blacklistedInEUAllowed
  type: boolean
- description: This option ensures that the system will only consider these airlines.
  name: excludedCarrierCodes
  type: array
- description: This option ensures that the system will only consider these airlines.
  name: includedCarrierCodes
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-carrierrestrictions-schema.json
slug: flight-availibilities-search-carrierrestrictions
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
title: CarrierRestrictions
---
