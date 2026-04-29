---
description: Program transition configuration.
layout: schema
name: UpdateProgramTransition
properties_list:
- description: ''
  name: DurationMillis
  type: object
- description: ''
  name: ScheduledStartTimeMillis
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-update-program-transition-schema.json
slug: mediatailor-api-update-program-transition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-update-program-transition-schema.json\",\n  \"title\": \"UpdateProgramTransition\",\n  \"description\": \"Program transition configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DurationMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The duration of the live program in seconds.\"\n        }\n      ]\n    },\n    \"ScheduledStartTimeMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The date and time that the program is scheduled to start, in epoch milliseconds.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-update-program-transition-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateProgramTransition
---
