---
description: UpdateProgramRequest schema from Amazon MediaTailor API
layout: schema
name: UpdateProgramRequest
properties_list:
- description: ''
  name: AdBreaks
  type: object
- description: ''
  name: ScheduleConfiguration
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-update-program-request-schema.json
slug: mediatailor-api-update-program-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-update-program-request-schema.json\",\n  \"title\": \"UpdateProgramRequest\",\n  \"description\": \"UpdateProgramRequest schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdBreaks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAdBreak\"\n        },\n        {\n          \"description\": \"The ad break configuration settings.\"\n        }\n      ]\n    },\n    \"ScheduleConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateProgramScheduleConfiguration\"\n        },\n        {\n          \"description\": \"The schedule configuration settings.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ScheduleConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-update-program-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateProgramRequest
---
