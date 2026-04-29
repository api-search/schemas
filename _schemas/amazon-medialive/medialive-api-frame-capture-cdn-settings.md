---
description: Frame Capture Cdn Settings
layout: schema
name: FrameCaptureCdnSettings
properties_list:
- description: ''
  name: FrameCaptureS3Settings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-frame-capture-cdn-settings-schema.json
slug: medialive-api-frame-capture-cdn-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-frame-capture-cdn-settings-schema.json\",\n  \"title\": \"FrameCaptureCdnSettings\",\n  \"description\": \"Frame Capture Cdn Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FrameCaptureS3Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameCaptureS3Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"frameCaptureS3Settings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-frame-capture-cdn-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: FrameCaptureCdnSettings
---
