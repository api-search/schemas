---
description: AnalysisResultLocations schema
layout: schema
name: AnalysisResultLocations
properties_list: []
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-analysis-result-locations-schema.json
slug: iot-events-analysis-result-locations
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-analysis-result-locations-schema.json\",\n  \"title\": \"AnalysisResultLocations\",\n  \"description\": \"AnalysisResultLocations schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"path\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AnalysisResultLocationPath\"\n          },\n          {\n            \"description\": \"A <a href=\\\"https://github.com/json-path/JsonPath\\\">JsonPath</a> expression that identifies the error field in your detector model.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information that you can use to locate the field in your detector model that the analysis result references.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-analysis-result-locations-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: AnalysisResultLocations
---
