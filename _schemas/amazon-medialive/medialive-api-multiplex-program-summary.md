---
description: Placeholder documentation for MultiplexProgramSummary
layout: schema
name: MultiplexProgramSummary
properties_list:
- description: ''
  name: ChannelId
  type: object
- description: ''
  name: ProgramName
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-program-summary-schema.json
slug: medialive-api-multiplex-program-summary
source_filename: medialive-api-multiplex-program-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-summary-schema.json\",\n  \"title\": \"MultiplexProgramSummary\",\n  \"description\": \"Placeholder documentation for MultiplexProgramSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelId\"\n          },\n          \"description\": \"The MediaLive Channel associated with the program.\"\n        }\n      ]\n    },\n    \"ProgramName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programName\"\n          },\n          \"description\": \"The name of the multiplex program.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-summary-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MultiplexProgramSummary
---
