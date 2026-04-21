---
description: Media is a digital content like image, video with associated text and description, several scales and some metadata can be provided also.
layout: schema
name: Amenity_Media
properties_list:
- description: media title
  name: title
  type: string
- description: href to display the original media.
  name: href
  type: string
- description: ''
  name: description
  type: object
- description: media type as per IANA (https://www.iana.org/assignments/media-types/media-types.xhtml)
  name: mediaType
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-amenity-media-schema.json
slug: seatmap-display-amenity-media
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
title: Amenity_Media
---
