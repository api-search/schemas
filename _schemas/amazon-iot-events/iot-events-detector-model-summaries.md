---
description: DetectorModelSummaries schema
layout: schema
name: DetectorModelSummaries
properties_list: []
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-detector-model-summaries-schema.json
slug: iot-events-detector-model-summaries
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-model-summaries-schema.json\",\n  \"title\": \"DetectorModelSummaries\",\n  \"description\": \"DetectorModelSummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"detectorModelName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DetectorModelName\"\n          },\n          {\n            \"description\": \"The name of the detector model.\"\n          }\n        ]\n      },\n      \"detectorModelDescription\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DetectorModelDescription\"\n          },\n          {\n            \"description\": \"A brief description of the detector model.\"\n          }\n        ]\n      },\n      \"creationTime\": {\n\
  \        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The time the detector model was created.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Information about the detector model.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-detector-model-summaries-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: DetectorModelSummaries
---
