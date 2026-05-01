---
description: ListEphemeridesResponse schema from Amazon Ground Station API
layout: schema
name: ListEphemeridesResponse
properties_list:
- description: ''
  name: ephemerides
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-list-ephemerides-response-schema.json
slug: ground-station-list-ephemerides-response
source_filename: ground-station-list-ephemerides-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-list-ephemerides-response-schema.json\",\n  \"title\": \"ListEphemeridesResponse\",\n  \"description\": \"ListEphemeridesResponse schema from Amazon Ground Station API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ephemerides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EphemeridesList\"\n        },\n        {\n          \"description\": \"List of ephemerides.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-list-ephemerides-response-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: ListEphemeridesResponse
---
