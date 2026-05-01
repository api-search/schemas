---
description: CreateJobForDevicesResponse schema from Amazon Panorama
layout: schema
name: CreateJobForDevicesResponse
properties_list:
- description: ''
  name: Jobs
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-create-job-for-devices-response-schema.json
slug: openapi-create-job-for-devices-response
source_filename: openapi-create-job-for-devices-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-job-for-devices-response-schema.json\",\n  \"title\": \"CreateJobForDevicesResponse\",\n  \"description\": \"CreateJobForDevicesResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Jobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobList\"\n        },\n        {\n          \"description\": \"A list of jobs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Jobs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-job-for-devices-response-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: CreateJobForDevicesResponse
---
