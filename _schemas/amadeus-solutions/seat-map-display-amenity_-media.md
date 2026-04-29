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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-amenity_-media-schema.json
slug: seat-map-display-amenity_-media
source_filename: seat-map-display-amenity_-media-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-amenity_-media-schema.json\",\n  \"title\": \"Amenity_Media\",\n  \"description\": \"Media is a digital content like image, video with associated text and description, several scales and some metadata can be provided also.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"media title\",\n      \"example\": \"My image title\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://pdt.multimediarepository.testing.amadeus.com/cmr/retrieve/hotel/69810B23CB8644A18AF760DC66BE41A6\",\n      \"description\": \"href to display the original media.\\n\"\n    },\n    \"description\": {\n      \"$ref\": \"#/definitions/QualifiedFreeText\"\n    },\n    \"mediaType\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"media type as per IANA (https://www.iana.org/assignments/media-types/media-types.xhtml)\",\n      \"enum\": [\n        \"application\",\n        \"audio\",\n        \"font\",\n        \"example\",\n        \"image\",\n        \"message\",\n        \"model\",\n        \"multipart\",\n        \"text\",\n        \"video\"\n      ],\n      \"example\": \"image\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-amenity_-media-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Amenity_Media
---
