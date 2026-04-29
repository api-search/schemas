---
description: AssociateTargetsWithJobResponse schema
layout: schema
name: AssociateTargetsWithJobResponse
properties_list:
- description: ''
  name: jobArn
  type: object
- description: ''
  name: jobId
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-associate-targets-with-job-response-schema.json
slug: iot-device-defender-associate-targets-with-job-response
source_filename: iot-device-defender-associate-targets-with-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-associate-targets-with-job-response-schema.json\",\n  \"title\": \"AssociateTargetsWithJobResponse\",\n  \"description\": \"AssociateTargetsWithJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobArn\"\n        },\n        {\n          \"description\": \"An ARN identifying the job.\"\n        }\n      ]\n    },\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The unique identifier you assigned to this job when it was created.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobDescription\"\
  \n        },\n        {\n          \"description\": \"A short text description of the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-associate-targets-with-job-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: AssociateTargetsWithJobResponse
---
