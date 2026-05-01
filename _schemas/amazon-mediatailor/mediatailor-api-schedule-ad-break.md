---
description: The schedule's ad break properties.
layout: schema
name: ScheduleAdBreak
properties_list:
- description: ''
  name: ApproximateDurationSeconds
  type: object
- description: ''
  name: ApproximateStartTime
  type: object
- description: ''
  name: SourceLocationName
  type: object
- description: ''
  name: VodSourceName
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-schedule-ad-break-schema.json
slug: mediatailor-api-schedule-ad-break
source_filename: mediatailor-api-schedule-ad-break-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-schedule-ad-break-schema.json\",\n  \"title\": \"ScheduleAdBreak\",\n  \"description\": \"The schedule's ad break properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApproximateDurationSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The approximate duration of the ad break, in seconds.\"\n        }\n      ]\n    },\n    \"ApproximateStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The approximate time that the ad will start playing.\"\n        }\n      ]\n    },\n    \"SourceLocationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"description\": \"The name of the source location containing the VOD source used for the ad break.\"\n        }\n      ]\n    },\n    \"VodSourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the VOD source used for the ad break.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-schedule-ad-break-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ScheduleAdBreak
---
