---
description: Placeholder documentation for ListReservationsResponse
layout: schema
name: ListReservationsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Reservations
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-list-reservations-response-schema.json
slug: medialive-api-list-reservations-response
source_filename: medialive-api-list-reservations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-reservations-response-schema.json\",\n  \"title\": \"ListReservationsResponse\",\n  \"description\": \"Placeholder documentation for ListReservationsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"Token to retrieve the next page of results\"\n        }\n      ]\n    },\n    \"Reservations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfReservation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reservations\"\n          },\n          \"description\": \"List of reservations\"\n   \
  \     }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-reservations-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListReservationsResponse
---
