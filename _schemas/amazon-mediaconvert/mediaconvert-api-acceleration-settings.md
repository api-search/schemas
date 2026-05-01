---
description: Accelerated transcoding can significantly speed up jobs with long, visually complex content.
layout: schema
name: AccelerationSettings
properties_list:
- description: ''
  name: Mode
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-acceleration-settings-schema.json
slug: mediaconvert-api-acceleration-settings
source_filename: mediaconvert-api-acceleration-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-acceleration-settings-schema.json\",\n  \"title\": \"AccelerationSettings\",\n  \"description\": \"Accelerated transcoding can significantly speed up jobs with long, visually complex content.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccelerationMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mode\"\n          },\n          \"description\": \"Specify the conditions when the service will run your job with accelerated transcoding.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Mode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-acceleration-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AccelerationSettings
---
