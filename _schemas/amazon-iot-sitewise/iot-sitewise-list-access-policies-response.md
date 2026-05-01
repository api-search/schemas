---
description: ListAccessPoliciesResponse schema
layout: schema
name: ListAccessPoliciesResponse
properties_list:
- description: ''
  name: accessPolicySummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-list-access-policies-response-schema.json
slug: iot-sitewise-list-access-policies-response
source_filename: iot-sitewise-list-access-policies-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-access-policies-response-schema.json\",\n  \"title\": \"ListAccessPoliciesResponse\",\n  \"description\": \"ListAccessPoliciesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessPolicySummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPolicySummaries\"\n        },\n        {\n          \"description\": \"A list that summarizes each access policy.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accessPolicySummaries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-access-policies-response-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: ListAccessPoliciesResponse
---
