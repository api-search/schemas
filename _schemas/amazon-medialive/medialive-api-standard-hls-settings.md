---
description: Standard Hls Settings
layout: schema
name: StandardHlsSettings
properties_list:
- description: ''
  name: AudioRenditionSets
  type: object
- description: ''
  name: M3u8Settings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-standard-hls-settings-schema.json
slug: medialive-api-standard-hls-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-standard-hls-settings-schema.json\",\n  \"title\": \"StandardHlsSettings\",\n  \"description\": \"Standard Hls Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioRenditionSets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioRenditionSets\"\n          },\n          \"description\": \"List all the audio groups that are used with the video output stream. Input all the audio GROUP-IDs that are associated to the video, separate by ','.\"\n        }\n      ]\n    },\n    \"M3u8Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M3u8Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"m3u8Settings\"\
  \n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"M3u8Settings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-standard-hls-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: StandardHlsSettings
---
