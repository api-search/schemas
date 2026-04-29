---
description: Schedule configuration parameters.
layout: schema
name: UpdateProgramScheduleConfiguration
properties_list:
- description: ''
  name: ClipRange
  type: object
- description: ''
  name: Transition
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-update-program-schedule-configuration-schema.json
slug: mediatailor-api-update-program-schedule-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-update-program-schedule-configuration-schema.json\",\n  \"title\": \"UpdateProgramScheduleConfiguration\",\n  \"description\": \"Schedule configuration parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClipRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClipRange\"\n        },\n        {\n          \"description\": \"Program clip range configuration.\"\n        }\n      ]\n    },\n    \"Transition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateProgramTransition\"\n        },\n        {\n          \"description\": \"Program transition configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-update-program-schedule-configuration-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateProgramScheduleConfiguration
---
