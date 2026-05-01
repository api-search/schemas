---
description: Frame Capture S3 Settings
layout: schema
name: FrameCaptureS3Settings
properties_list:
- description: ''
  name: CannedAcl
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-frame-capture-s3-settings-schema.json
slug: medialive-api-frame-capture-s3-settings
source_filename: medialive-api-frame-capture-s3-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-frame-capture-s3-settings-schema.json\",\n  \"title\": \"FrameCaptureS3Settings\",\n  \"description\": \"Frame Capture S3 Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CannedAcl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3CannedAcl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cannedAcl\"\n          },\n          \"description\": \"Specify the canned ACL to apply to each S3 request. Defaults to none.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-frame-capture-s3-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: FrameCaptureS3Settings
---
