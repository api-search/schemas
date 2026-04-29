---
description: GetBehaviorModelTrainingSummariesResponse schema
layout: schema
name: GetBehaviorModelTrainingSummariesResponse
properties_list:
- description: ''
  name: summaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-get-behavior-model-training-summaries-response-schema.json
slug: iot-core-get-behavior-model-training-summaries-response
source_filename: iot-core-get-behavior-model-training-summaries-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-behavior-model-training-summaries-response-schema.json\",\n  \"title\": \"GetBehaviorModelTrainingSummariesResponse\",\n  \"description\": \"GetBehaviorModelTrainingSummariesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"summaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BehaviorModelTrainingSummaries\"\n        },\n        {\n          \"description\": \" A list of all ML Detect behaviors and their model status for a given Security Profile. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" A token that can be used to retrieve the next set of results, or <code>null</code> if there are\
  \ no additional results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-get-behavior-model-training-summaries-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: GetBehaviorModelTrainingSummariesResponse
---
