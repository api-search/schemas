---
description: CreateProgramResponse schema from Amazon MediaTailor API
layout: schema
name: CreateProgramResponse
properties_list:
- description: ''
  name: AdBreaks
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: ChannelName
  type: object
- description: ''
  name: ClipRange
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: DurationMillis
  type: object
- description: ''
  name: LiveSourceName
  type: object
- description: ''
  name: ProgramName
  type: object
- description: ''
  name: ScheduledStartTime
  type: object
- description: ''
  name: SourceLocationName
  type: object
- description: ''
  name: VodSourceName
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-create-program-response-schema.json
slug: mediatailor-api-create-program-response
source_filename: mediatailor-api-create-program-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-program-response-schema.json\",\n  \"title\": \"CreateProgramResponse\",\n  \"description\": \"CreateProgramResponse schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdBreaks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAdBreak\"\n        },\n        {\n          \"description\": \"The ad break configuration settings.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The ARN to assign to the program.\"\n        }\n      ]\n    },\n    \"ChannelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n\
  \          \"description\": \"The name to assign to the channel for this program.\"\n        }\n      ]\n    },\n    \"ClipRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClipRange\"\n        },\n        {\n          \"description\": \"The clip range configuration settings.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The time the program was created.\"\n        }\n      ]\n    },\n    \"DurationMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The duration of the live program in milliseconds.\"\n        }\n      ]\n    },\n    \"LiveSourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of\
  \ the LiveSource for this Program.\"\n        }\n      ]\n    },\n    \"ProgramName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name to assign to this program.\"\n        }\n      ]\n    },\n    \"ScheduledStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The scheduled start time for this Program.\"\n        }\n      ]\n    },\n    \"SourceLocationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name to assign to the source location for this program.\"\n        }\n      ]\n    },\n    \"VodSourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name that's used to refer to\
  \ a VOD source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-program-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateProgramResponse
---
