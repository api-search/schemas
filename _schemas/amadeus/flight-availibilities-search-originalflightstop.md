---
description: details of stops for direct or change of gauge flights
layout: schema
name: OriginalFlightStop
properties_list:
- description: '[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)'
  name: iataCode
  type: string
- description: stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M
  name: duration
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-originalflightstop-schema.json
slug: flight-availibilities-search-originalflightstop
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
title: OriginalFlightStop
---
