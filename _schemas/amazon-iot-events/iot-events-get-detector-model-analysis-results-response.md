---
description: GetDetectorModelAnalysisResultsResponse schema
layout: schema
name: GetDetectorModelAnalysisResultsResponse
properties_list:
- description: ''
  name: analysisResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-get-detector-model-analysis-results-response-schema.json
slug: iot-events-get-detector-model-analysis-results-response
source_filename: iot-events-get-detector-model-analysis-results-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-get-detector-model-analysis-results-response-schema.json\",\n  \"title\": \"GetDetectorModelAnalysisResultsResponse\",\n  \"description\": \"GetDetectorModelAnalysisResultsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"analysisResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalysisResults\"\n        },\n        {\n          \"description\": \"Contains information about one or more analysis results.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token that you can use to return the next set of results, or <code>null</code> if there are no more results.\"\n        }\n      ]\n   \
  \ }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-get-detector-model-analysis-results-response-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: GetDetectorModelAnalysisResultsResponse
---
