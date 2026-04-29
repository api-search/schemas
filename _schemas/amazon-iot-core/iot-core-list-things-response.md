---
description: The output from the ListThings operation.
layout: schema
name: ListThingsResponse
properties_list:
- description: ''
  name: things
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-things-response-schema.json
slug: iot-core-list-things-response
source_filename: iot-core-list-things-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-things-response-schema.json\",\n  \"title\": \"ListThingsResponse\",\n  \"description\": \"The output from the ListThings operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"things\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingAttributeList\"\n        },\n        {\n          \"description\": \"The things.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to use to get the next set of results. Will not be returned if operation has returned all results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-things-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: ListThingsResponse
---
