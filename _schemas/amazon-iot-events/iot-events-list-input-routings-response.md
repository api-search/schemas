---
description: ListInputRoutingsResponse schema
layout: schema
name: ListInputRoutingsResponse
properties_list:
- description: ''
  name: routedResources
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-list-input-routings-response-schema.json
slug: iot-events-list-input-routings-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-list-input-routings-response-schema.json\",\n  \"title\": \"ListInputRoutingsResponse\",\n  \"description\": \"ListInputRoutingsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"routedResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoutedResources\"\n        },\n        {\n          \"description\": \" Summary information about the routed resources. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" The token that you can use to return the next set of results, or <code>null</code> if there are no more results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-list-input-routings-response-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: ListInputRoutingsResponse
---
