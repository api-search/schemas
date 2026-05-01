---
description: CreateJobForDevicesRequest schema from Amazon Panorama
layout: schema
name: CreateJobForDevicesRequest
properties_list:
- description: ''
  name: DeviceIds
  type: object
- description: ''
  name: DeviceJobConfig
  type: object
- description: ''
  name: JobType
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-create-job-for-devices-request-schema.json
slug: openapi-create-job-for-devices-request
source_filename: openapi-create-job-for-devices-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-job-for-devices-request-schema.json\",\n  \"title\": \"CreateJobForDevicesRequest\",\n  \"description\": \"CreateJobForDevicesRequest schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeviceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceIdList\"\n        },\n        {\n          \"description\": \"ID of target device.\"\n        }\n      ]\n    },\n    \"DeviceJobConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceJobConfig\"\n        },\n        {\n          \"description\": \"Configuration settings for a software update job.\"\n        }\n      ]\n    },\n    \"JobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobType\"\n        },\n\
  \        {\n          \"description\": \"The type of job to run.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DeviceIds\",\n    \"JobType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-job-for-devices-request-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: CreateJobForDevicesRequest
---
