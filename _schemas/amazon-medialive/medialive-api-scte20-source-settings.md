---
description: Scte20 Source Settings
layout: schema
name: Scte20SourceSettings
properties_list:
- description: ''
  name: Convert608To708
  type: object
- description: ''
  name: Source608ChannelNumber
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte20-source-settings-schema.json
slug: medialive-api-scte20-source-settings
source_filename: medialive-api-scte20-source-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte20-source-settings-schema.json\",\n  \"title\": \"Scte20SourceSettings\",\n  \"description\": \"Scte20 Source Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Convert608To708\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte20Convert608To708\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"convert608To708\"\n          },\n          \"description\": \"If upconvert, 608 data is both passed through via the \\\"608 compatibility bytes\\\" fields of the 708 wrapper as well as translated into 708. 708 data present in the source content will be discarded.\"\n        }\n      ]\n    },\n    \"Source608ChannelNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max4\"\n   \
  \     },\n        {\n          \"xml\": {\n            \"name\": \"source608ChannelNumber\"\n          },\n          \"description\": \"Specifies the 608/708 channel number within the video track from which to extract captions. Unused for passthrough.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte20-source-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Scte20SourceSettings
---
