---
description: CreateProgramRequest schema from Amazon MediaTailor API
layout: schema
name: CreateProgramRequest
properties_list:
- description: ''
  name: AdBreaks
  type: object
- description: ''
  name: LiveSourceName
  type: object
- description: ''
  name: ScheduleConfiguration
  type: object
- description: ''
  name: SourceLocationName
  type: object
- description: ''
  name: VodSourceName
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-create-program-request-schema.json
slug: mediatailor-api-create-program-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-program-request-schema.json\",\n  \"title\": \"CreateProgramRequest\",\n  \"description\": \"CreateProgramRequest schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdBreaks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAdBreak\"\n        },\n        {\n          \"description\": \"The ad break configuration settings.\"\n        }\n      ]\n    },\n    \"LiveSourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the LiveSource for this Program.\"\n        }\n      ]\n    },\n    \"ScheduleConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleConfiguration\"\
  \n        },\n        {\n          \"description\": \"The schedule configuration settings.\"\n        }\n      ]\n    },\n    \"SourceLocationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the source location.\"\n        }\n      ]\n    },\n    \"VodSourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name that's used to refer to a VOD source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ScheduleConfiguration\",\n    \"SourceLocationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-program-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateProgramRequest
---
