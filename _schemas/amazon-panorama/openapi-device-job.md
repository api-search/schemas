---
description: A job that runs on a device.
layout: schema
name: DeviceJob
properties_list:
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: DeviceId
  type: object
- description: ''
  name: DeviceName
  type: object
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobType
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-device-job-schema.json
slug: openapi-device-job
source_filename: openapi-device-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-device-job-schema.json\",\n  \"title\": \"DeviceJob\",\n  \"description\": \"A job that runs on a device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedTime\"\n        },\n        {\n          \"description\": \"When the job was created.\"\n        }\n      ]\n    },\n    \"DeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceId\"\n        },\n        {\n          \"description\": \"The ID of the target device.\"\n        }\n      ]\n    },\n    \"DeviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceName\"\n        },\n        {\n          \"description\": \"The name of the target device\"\n        }\n\
  \      ]\n    },\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The job's ID.\"\n        }\n      ]\n    },\n    \"JobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobType\"\n        },\n        {\n          \"description\": \"The job's type.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-device-job-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: DeviceJob
---
