---
description: Dvb Sub Source Settings
layout: schema
name: DvbSubSourceSettings
properties_list:
- description: ''
  name: OcrLanguage
  type: object
- description: ''
  name: Pid
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-dvb-sub-source-settings-schema.json
slug: medialive-api-dvb-sub-source-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-dvb-sub-source-settings-schema.json\",\n  \"title\": \"DvbSubSourceSettings\",\n  \"description\": \"Dvb Sub Source Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OcrLanguage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSubOcrLanguage\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ocrLanguage\"\n          },\n          \"description\": \"If you will configure a WebVTT caption description that references this caption selector, use this field to\\nprovide the language to consider when translating the image-based source to text.\"\n        }\n      ]\n    },\n    \"Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n \
  \           \"name\": \"pid\"\n          },\n          \"description\": \"When using DVB-Sub with Burn-In or SMPTE-TT, use this PID for the source content. Unused for DVB-Sub passthrough. All DVB-Sub content is passed through, regardless of selectors.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-dvb-sub-source-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DvbSubSourceSettings
---
