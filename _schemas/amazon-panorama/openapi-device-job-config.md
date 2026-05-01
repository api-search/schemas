---
description: A job's configuration.
layout: schema
name: DeviceJobConfig
properties_list:
- description: ''
  name: OTAJobConfig
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-device-job-config-schema.json
slug: openapi-device-job-config
source_filename: openapi-device-job-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-device-job-config-schema.json\",\n  \"title\": \"DeviceJobConfig\",\n  \"description\": \"A job's configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OTAJobConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OTAJobConfig\"\n        },\n        {\n          \"description\": \"A configuration for an over-the-air (OTA) upgrade. Required for OTA jobs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-device-job-config-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: DeviceJobConfig
---
