---
description: Frame Capture Settings
layout: schema
name: FrameCaptureSettings
properties_list:
- description: ''
  name: CaptureInterval
  type: object
- description: ''
  name: CaptureIntervalUnits
  type: object
- description: ''
  name: TimecodeBurninSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-frame-capture-settings-schema.json
slug: medialive-api-frame-capture-settings
source_filename: medialive-api-frame-capture-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-frame-capture-settings-schema.json\",\n  \"title\": \"FrameCaptureSettings\",\n  \"description\": \"Frame Capture Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CaptureInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max3600000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captureInterval\"\n          },\n          \"description\": \"The frequency at which to capture frames for inclusion in the output. May be specified in either seconds or milliseconds, as specified by captureIntervalUnits.\"\n        }\n      ]\n    },\n    \"CaptureIntervalUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameCaptureIntervalUnit\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"captureIntervalUnits\"\n          },\n          \"description\": \"Unit for the frame capture interval.\"\n        }\n      ]\n    },\n    \"TimecodeBurninSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimecodeBurninSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timecodeBurninSettings\"\n          },\n          \"description\": \"Timecode burn-in settings\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-frame-capture-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: FrameCaptureSettings
---
