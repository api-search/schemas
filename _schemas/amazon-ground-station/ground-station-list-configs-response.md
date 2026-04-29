---
description: <p/>
layout: schema
name: ListConfigsResponse
properties_list:
- description: ''
  name: configList
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-list-configs-response-schema.json
slug: ground-station-list-configs-response
source_filename: ground-station-list-configs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-list-configs-response-schema.json\",\n  \"title\": \"ListConfigsResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigList\"\n        },\n        {\n          \"description\": \"List of <code>Config</code> items.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Next token returned in the response of a previous <code>ListConfigs</code> call. Used to get the next page of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-list-configs-response-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: ListConfigsResponse
---
