---
description: Schedule configuration parameters. A channel must be stopped before changes can be made to the schedule.
layout: schema
name: ScheduleConfiguration
properties_list:
- description: ''
  name: ClipRange
  type: object
- description: ''
  name: Transition
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-schedule-configuration-schema.json
slug: mediatailor-api-schedule-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-schedule-configuration-schema.json\",\n  \"title\": \"ScheduleConfiguration\",\n  \"description\": \"Schedule configuration parameters. A channel must be stopped before changes can be made to the schedule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClipRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClipRange\"\n        },\n        {\n          \"description\": \"Program clip range configuration.\"\n        }\n      ]\n    },\n    \"Transition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Transition\"\n        },\n        {\n          \"description\": \"Program transition configurations.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Transition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-schedule-configuration-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ScheduleConfiguration
---
