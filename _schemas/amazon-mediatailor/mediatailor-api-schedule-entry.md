---
description: The properties for a schedule.
layout: schema
name: ScheduleEntry
properties_list:
- description: ''
  name: ApproximateDurationSeconds
  type: object
- description: ''
  name: ApproximateStartTime
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: ChannelName
  type: object
- description: ''
  name: LiveSourceName
  type: object
- description: ''
  name: ProgramName
  type: object
- description: ''
  name: ScheduleAdBreaks
  type: object
- description: ''
  name: ScheduleEntryType
  type: object
- description: ''
  name: SourceLocationName
  type: object
- description: ''
  name: VodSourceName
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-schedule-entry-schema.json
slug: mediatailor-api-schedule-entry
source_filename: mediatailor-api-schedule-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-schedule-entry-schema.json\",\n  \"title\": \"ScheduleEntry\",\n  \"description\": \"The properties for a schedule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApproximateDurationSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The approximate duration of this program, in seconds.\"\n        }\n      ]\n    },\n    \"ApproximateStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The approximate time that the program will start playing.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n\
  \        },\n        {\n          \"description\": \"The ARN of the program.\"\n        }\n      ]\n    },\n    \"ChannelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the channel that uses this schedule.\"\n        }\n      ]\n    },\n    \"LiveSourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the live source used for the program.\"\n        }\n      ]\n    },\n    \"ProgramName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the program.\"\n        }\n      ]\n    },\n    \"ScheduleAdBreaks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfScheduleAdBreak\"\n        },\n        {\n          \"description\": \"The\
  \ schedule's ad break properties.\"\n        }\n      ]\n    },\n    \"ScheduleEntryType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleEntryType\"\n        },\n        {\n          \"description\": \"The type of schedule entry.\"\n        }\n      ]\n    },\n    \"SourceLocationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the source location.\"\n        }\n      ]\n    },\n    \"VodSourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the VOD source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\",\n    \"ChannelName\",\n    \"ProgramName\",\n    \"SourceLocationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-schedule-entry-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ScheduleEntry
---
