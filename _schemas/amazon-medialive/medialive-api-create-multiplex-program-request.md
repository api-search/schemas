---
description: A request to create a program in a multiplex.
layout: schema
name: CreateMultiplexProgramRequest
properties_list:
- description: ''
  name: MultiplexProgramSettings
  type: object
- description: ''
  name: ProgramName
  type: object
- description: ''
  name: RequestId
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-create-multiplex-program-request-schema.json
slug: medialive-api-create-multiplex-program-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-multiplex-program-request-schema.json\",\n  \"title\": \"CreateMultiplexProgramRequest\",\n  \"description\": \"A request to create a program in a multiplex.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MultiplexProgramSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexProgramSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexProgramSettings\"\n          },\n          \"description\": \"The settings for this multiplex program.\"\n        }\n      ]\n    },\n    \"ProgramName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programName\"\n          },\n          \"description\"\
  : \"Name of multiplex program.\"\n        }\n      ]\n    },\n    \"RequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"requestId\"\n          },\n          \"description\": \"Unique request ID. This prevents retries from creating multiple\\nresources.\\n\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RequestId\",\n    \"MultiplexProgramSettings\",\n    \"ProgramName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-create-multiplex-program-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateMultiplexProgramRequest
---
