---
description: ListInputRoutingsRequest schema
layout: schema
name: ListInputRoutingsRequest
properties_list:
- description: ''
  name: inputIdentifier
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-list-input-routings-request-schema.json
slug: iot-events-list-input-routings-request
source_filename: iot-events-list-input-routings-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-list-input-routings-request-schema.json\",\n  \"title\": \"ListInputRoutingsRequest\",\n  \"description\": \"ListInputRoutingsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputIdentifier\"\n        },\n        {\n          \"description\": \" The identifer of the routed input. \"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \" The maximum number of results to be returned per request. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n    \
  \    },\n        {\n          \"description\": \" The token that you can use to return the next set of results. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-list-input-routings-request-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: ListInputRoutingsRequest
---
