---
description: Audio Dolby EDecode
layout: schema
name: AudioDolbyEDecode
properties_list:
- description: ''
  name: ProgramSelection
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-dolby-e-decode-schema.json
slug: medialive-api-audio-dolby-e-decode
source_filename: medialive-api-audio-dolby-e-decode-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-dolby-e-decode-schema.json\",\n  \"title\": \"AudioDolbyEDecode\",\n  \"description\": \"Audio Dolby EDecode\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProgramSelection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DolbyEProgramSelection\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programSelection\"\n          },\n          \"description\": \"Applies only to Dolby E. Enter the program ID (according to the metadata in the audio) of the Dolby E program to extract from the specified track. One program extracted per audio selector. To select multiple programs, create multiple selectors with the same Track and different Program numbers. \\u201cAll channels\\u201d means to ignore the program IDs and include all the\
  \ channels in this selector; useful if metadata is known to be incorrect.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ProgramSelection\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-dolby-e-decode-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioDolbyEDecode
---
