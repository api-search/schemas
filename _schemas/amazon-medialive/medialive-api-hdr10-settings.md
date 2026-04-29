---
description: Hdr10 Settings
layout: schema
name: Hdr10Settings
properties_list:
- description: ''
  name: MaxCll
  type: object
- description: ''
  name: MaxFall
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-hdr10-settings-schema.json
slug: medialive-api-hdr10-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hdr10-settings-schema.json\",\n  \"title\": \"Hdr10Settings\",\n  \"description\": \"Hdr10 Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxCll\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max32768\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxCll\"\n          },\n          \"description\": \"Maximum Content Light Level\\nAn integer metadata value defining the maximum light level, in nits,\\nof any single pixel within an encoded HDR video stream or file.\"\n        }\n      ]\n    },\n    \"MaxFall\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max32768\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxFall\"\n          },\n\
  \          \"description\": \"Maximum Frame Average Light Level\\nAn integer metadata value defining the maximum average light level, in nits,\\nfor any single frame within an encoded HDR video stream or file.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hdr10-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Hdr10Settings
---
