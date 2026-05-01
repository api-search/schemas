---
description: <p/>
layout: schema
name: ListGroundStationsResponse
properties_list:
- description: ''
  name: groundStationList
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-list-ground-stations-response-schema.json
slug: ground-station-list-ground-stations-response
source_filename: ground-station-list-ground-stations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-list-ground-stations-response-schema.json\",\n  \"title\": \"ListGroundStationsResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groundStationList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroundStationList\"\n        },\n        {\n          \"description\": \"List of ground stations.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Next token that can be supplied in the next call to get the next page of ground stations.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-list-ground-stations-response-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: ListGroundStationsResponse
---
