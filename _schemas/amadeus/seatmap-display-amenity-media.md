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
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Amenity_Media\",\n  \"description\": \"Media is a digital content like image, video with associated text and description, several scales and some metadata can be provided also.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"media title\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"href to display the original media.\\n\"\n    },\n    \"description\": {\n      \"$ref\": \"#/definitions/QualifiedFreeText\"\n    },\n    \"mediaType\": {\n      \"type\": \"string\",\n      \"description\": \"media type as per IANA (https://www.iana.org/assignments/media-types/media-types.xhtml)\",\n      \"enum\": [\n        \"application\",\n        \"audio\",\n        \"font\",\n        \"example\",\n        \"image\",\n        \"message\",\n        \"model\",\n        \"multipart\"\
  ,\n        \"text\",\n        \"video\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-amenity-media-schema.json
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
