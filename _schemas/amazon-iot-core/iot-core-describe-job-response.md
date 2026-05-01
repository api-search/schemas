---
description: DescribeJobResponse schema
layout: schema
name: DescribeJobResponse
properties_list:
- description: ''
  name: documentSource
  type: object
- description: ''
  name: job
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-describe-job-response-schema.json
slug: iot-core-describe-job-response
source_filename: iot-core-describe-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-job-response-schema.json\",\n  \"title\": \"DescribeJobResponse\",\n  \"description\": \"DescribeJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"documentSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobDocumentSource\"\n        },\n        {\n          \"description\": \"An S3 link to the job document.\"\n        }\n      ]\n    },\n    \"job\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Job\"\n        },\n        {\n          \"description\": \"Information about the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-job-response-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: DescribeJobResponse
---
