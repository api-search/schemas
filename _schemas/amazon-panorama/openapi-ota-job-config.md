---
description: An over-the-air update (OTA) job configuration.
layout: schema
name: OTAJobConfig
properties_list:
- description: ''
  name: AllowMajorVersionUpdate
  type: object
- description: ''
  name: ImageVersion
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-ota-job-config-schema.json
slug: openapi-ota-job-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-ota-job-config-schema.json\",\n  \"title\": \"OTAJobConfig\",\n  \"description\": \"An over-the-air update (OTA) job configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AllowMajorVersionUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether to apply the update if it is a major version change.\"\n        }\n      ]\n    },\n    \"ImageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageVersion\"\n        },\n        {\n          \"description\": \"The target version of the device software.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ImageVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-ota-job-config-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: OTAJobConfig
---
