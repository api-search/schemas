---
description: ListIndicesResponse schema
layout: schema
name: ListIndicesResponse
properties_list:
- description: ''
  name: indexNames
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-indices-response-schema.json
slug: iot-core-list-indices-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-indices-response-schema.json\",\n  \"title\": \"ListIndicesResponse\",\n  \"description\": \"ListIndicesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"indexNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IndexNamesList\"\n        },\n        {\n          \"description\": \"The index names.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token used to get the next set of results, or <code>null</code> if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-indices-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: ListIndicesResponse
---
