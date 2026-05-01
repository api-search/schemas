---
description: Contains information that you can use to locate the field in your detector model that the analysis result references.
layout: schema
name: AnalysisResultLocation
properties_list:
- description: ''
  name: path
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-analysis-result-location-schema.json
slug: iot-events-analysis-result-location
source_filename: iot-events-analysis-result-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-analysis-result-location-schema.json\",\n  \"title\": \"AnalysisResultLocation\",\n  \"description\": \"Contains information that you can use to locate the field in your detector model that the analysis result references.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalysisResultLocationPath\"\n        },\n        {\n          \"description\": \"A <a href=\\\"https://github.com/json-path/JsonPath\\\">JsonPath</a> expression that identifies the error field in your detector model.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-analysis-result-location-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: AnalysisResultLocation
---
