---
description: DescribeDetectorModelAnalysisResponse schema
layout: schema
name: DescribeDetectorModelAnalysisResponse
properties_list:
- description: ''
  name: status
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-describe-detector-model-analysis-response-schema.json
slug: iot-events-describe-detector-model-analysis-response
source_filename: iot-events-describe-detector-model-analysis-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-describe-detector-model-analysis-response-schema.json\",\n  \"title\": \"DescribeDetectorModelAnalysisResponse\",\n  \"description\": \"DescribeDetectorModelAnalysisResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalysisStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the analysis activity. The status can be one of the following values:</p> <ul> <li> <p> <code>RUNNING</code> - AWS IoT Events is analyzing your detector model. This process can take several minutes to complete.</p> </li> <li> <p> <code>COMPLETE</code> - AWS IoT Events finished analyzing your detector model.</p> </li> <li> <p> <code>FAILED</code> - AWS IoT Events couldn't analyze your detector\
  \ model. Try again later.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-describe-detector-model-analysis-response-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: DescribeDetectorModelAnalysisResponse
---
