---
description: ListGatewaysResponse schema
layout: schema
name: ListGatewaysResponse
properties_list:
- description: ''
  name: gatewaySummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-list-gateways-response-schema.json
slug: iot-sitewise-list-gateways-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-gateways-response-schema.json\",\n  \"title\": \"ListGatewaysResponse\",\n  \"description\": \"ListGatewaysResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gatewaySummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewaySummaries\"\n        },\n        {\n          \"description\": \"A list that summarizes each gateway.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"gatewaySummaries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-gateways-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: ListGatewaysResponse
---
