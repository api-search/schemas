---
description: Returns information about the latest device job.
layout: schema
name: LatestDeviceJob
properties_list:
- description: ''
  name: ImageVersion
  type: object
- description: ''
  name: JobType
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-latest-device-job-schema.json
slug: openapi-latest-device-job
source_filename: openapi-latest-device-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-latest-device-job-schema.json\",\n  \"title\": \"LatestDeviceJob\",\n  \"description\": \"Returns information about the latest device job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ImageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageVersion\"\n        },\n        {\n          \"description\": \"The target version of the device software.\"\n        }\n      ]\n    },\n    \"JobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobType\"\n        },\n        {\n          \"description\": \"The job's type.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateProgress\"\n        },\n        {\n          \"description\": \"Status of\
  \ the latest device job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-latest-device-job-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: LatestDeviceJob
---
