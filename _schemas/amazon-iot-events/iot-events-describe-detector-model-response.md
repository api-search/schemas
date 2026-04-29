---
description: DescribeDetectorModelResponse schema
layout: schema
name: DescribeDetectorModelResponse
properties_list:
- description: ''
  name: detectorModel
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-describe-detector-model-response-schema.json
slug: iot-events-describe-detector-model-response
source_filename: iot-events-describe-detector-model-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-describe-detector-model-response-schema.json\",\n  \"title\": \"DescribeDetectorModelResponse\",\n  \"description\": \"DescribeDetectorModelResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detectorModel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorModel\"\n        },\n        {\n          \"description\": \"Information about the detector model.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-describe-detector-model-response-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: DescribeDetectorModelResponse
---
