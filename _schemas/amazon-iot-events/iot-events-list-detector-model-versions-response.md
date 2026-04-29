---
description: ListDetectorModelVersionsResponse schema
layout: schema
name: ListDetectorModelVersionsResponse
properties_list:
- description: ''
  name: detectorModelVersionSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-list-detector-model-versions-response-schema.json
slug: iot-events-list-detector-model-versions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-list-detector-model-versions-response-schema.json\",\n  \"title\": \"ListDetectorModelVersionsResponse\",\n  \"description\": \"ListDetectorModelVersionsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detectorModelVersionSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModelVersionSummaries\"\n        },\n        {\n          \"description\": \"Summary information about the detector model versions.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token that you can use to return the next set of results, or <code>null</code> if there are no more results.\"\n        }\n     \
  \ ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-list-detector-model-versions-response-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: ListDetectorModelVersionsResponse
---
