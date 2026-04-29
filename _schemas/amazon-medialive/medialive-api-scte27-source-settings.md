---
description: Scte27 Source Settings
layout: schema
name: Scte27SourceSettings
properties_list:
- description: ''
  name: OcrLanguage
  type: object
- description: ''
  name: Pid
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte27-source-settings-schema.json
slug: medialive-api-scte27-source-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte27-source-settings-schema.json\",\n  \"title\": \"Scte27SourceSettings\",\n  \"description\": \"Scte27 Source Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OcrLanguage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte27OcrLanguage\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ocrLanguage\"\n          },\n          \"description\": \"If you will configure a WebVTT caption description that references this caption selector, use this field to\\nprovide the language to consider when translating the image-based source to text.\"\n        }\n      ]\n    },\n    \"Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n   \
  \         \"name\": \"pid\"\n          },\n          \"description\": \"The pid field is used in conjunction with the caption selector languageCode field as follows:\\n  - Specify PID and Language: Extracts captions from that PID; the language is \\\"informational\\\".\\n  - Specify PID and omit Language: Extracts the specified PID.\\n  - Omit PID and specify Language: Extracts the specified language, whichever PID that happens to be.\\n  - Omit PID and omit Language: Valid only if source is DVB-Sub that is being passed through; all languages will be passed through.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte27-source-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Scte27SourceSettings
---
