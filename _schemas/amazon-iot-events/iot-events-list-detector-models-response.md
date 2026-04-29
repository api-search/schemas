---
description: ListDetectorModelsResponse schema
layout: schema
name: ListDetectorModelsResponse
properties_list:
- description: ''
  name: detectorModelSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-list-detector-models-response-schema.json
slug: iot-events-list-detector-models-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-list-detector-models-response-schema.json\",\n  \"title\": \"ListDetectorModelsResponse\",\n  \"description\": \"ListDetectorModelsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detectorModelSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelSummaries\"\n        },\n        {\n          \"description\": \"Summary information about the detector models.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token that you can use to return the next set of results, or <code>null</code> if there are no more results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-list-detector-models-response-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: ListDetectorModelsResponse
---
