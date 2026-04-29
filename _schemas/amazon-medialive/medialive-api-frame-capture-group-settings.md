---
description: Frame Capture Group Settings
layout: schema
name: FrameCaptureGroupSettings
properties_list:
- description: ''
  name: Destination
  type: object
- description: ''
  name: FrameCaptureCdnSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-frame-capture-group-settings-schema.json
slug: medialive-api-frame-capture-group-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-frame-capture-group-settings-schema.json\",\n  \"title\": \"FrameCaptureGroupSettings\",\n  \"description\": \"Frame Capture Group Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputLocationRef\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destination\"\n          },\n          \"description\": \"The destination for the frame capture files. Either the URI for an Amazon S3 bucket and object, plus a file name prefix (for example, s3ssl://sportsDelivery/highlights/20180820/curling-) or the URI for a MediaStore container, plus a file name prefix (for example, mediastoressl://sportsDelivery/20180820/curling-). The final file names consist of the prefix from\
  \ the destination field (for example, \\\"curling-\\\") + name modifier + the counter (5 digits, starting from 00001) + extension (which is always .jpg).  For example, curling-low.00001.jpg\"\n        }\n      ]\n    },\n    \"FrameCaptureCdnSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameCaptureCdnSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"frameCaptureCdnSettings\"\n          },\n          \"description\": \"Parameters that control interactions with the CDN.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Destination\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-frame-capture-group-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: FrameCaptureGroupSettings
---
