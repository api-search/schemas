---
description: Frame Capture Output Settings
layout: schema
name: FrameCaptureOutputSettings
properties_list:
- description: ''
  name: NameModifier
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-frame-capture-output-settings-schema.json
slug: medialive-api-frame-capture-output-settings
source_filename: medialive-api-frame-capture-output-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-frame-capture-output-settings-schema.json\",\n  \"title\": \"FrameCaptureOutputSettings\",\n  \"description\": \"Frame Capture Output Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NameModifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nameModifier\"\n          },\n          \"description\": \"Required if the output group contains more than one output. This modifier forms part of the output file name.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-frame-capture-output-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: FrameCaptureOutputSettings
---
