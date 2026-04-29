---
description: Hls Settings
layout: schema
name: HlsSettings
properties_list:
- description: ''
  name: AudioOnlyHlsSettings
  type: object
- description: ''
  name: Fmp4HlsSettings
  type: object
- description: ''
  name: FrameCaptureHlsSettings
  type: object
- description: ''
  name: StandardHlsSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-hls-settings-schema.json
slug: medialive-api-hls-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-settings-schema.json\",\n  \"title\": \"HlsSettings\",\n  \"description\": \"Hls Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioOnlyHlsSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioOnlyHlsSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioOnlyHlsSettings\"\n          }\n        }\n      ]\n    },\n    \"Fmp4HlsSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Fmp4HlsSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fmp4HlsSettings\"\n          }\n        }\n      ]\n    },\n    \"FrameCaptureHlsSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameCaptureHlsSettings\"\n \
  \       },\n        {\n          \"xml\": {\n            \"name\": \"frameCaptureHlsSettings\"\n          }\n        }\n      ]\n    },\n    \"StandardHlsSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StandardHlsSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"standardHlsSettings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsSettings
---
