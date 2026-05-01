---
description: ListPortalsResponse schema
layout: schema
name: ListPortalsResponse
properties_list:
- description: ''
  name: portalSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-list-portals-response-schema.json
slug: iot-sitewise-list-portals-response
source_filename: iot-sitewise-list-portals-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-portals-response-schema.json\",\n  \"title\": \"ListPortalsResponse\",\n  \"description\": \"ListPortalsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portalSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortalSummaries\"\n        },\n        {\n          \"description\": \"A list that summarizes each portal.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-portals-response-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: ListPortalsResponse
---
