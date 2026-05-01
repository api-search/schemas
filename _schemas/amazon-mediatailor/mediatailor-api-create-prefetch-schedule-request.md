---
description: CreatePrefetchScheduleRequest schema from Amazon MediaTailor API
layout: schema
name: CreatePrefetchScheduleRequest
properties_list:
- description: ''
  name: Consumption
  type: object
- description: ''
  name: Retrieval
  type: object
- description: ''
  name: StreamId
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-create-prefetch-schedule-request-schema.json
slug: mediatailor-api-create-prefetch-schedule-request
source_filename: mediatailor-api-create-prefetch-schedule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-prefetch-schedule-request-schema.json\",\n  \"title\": \"CreatePrefetchScheduleRequest\",\n  \"description\": \"CreatePrefetchScheduleRequest schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Consumption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrefetchConsumption\"\n        },\n        {\n          \"description\": \"The configuration settings for MediaTailor's <i>consumption</i> of the prefetched ads from the ad decision server. Each consumption configuration contains an end time and an optional start time that define the <i>consumption window</i>. Prefetch schedules automatically expire no earlier than seven days after the end time.\"\n        }\n      ]\n    },\n    \"Retrieval\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/PrefetchRetrieval\"\n        },\n        {\n          \"description\": \"The configuration settings for retrieval of prefetched ads from the ad decision server. Only one set of prefetched ads will be retrieved and subsequently consumed for each ad break.\"\n        }\n      ]\n    },\n    \"StreamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"An optional stream identifier that MediaTailor uses to prefetch ads for multiple streams that use the same playback configuration. If <code>StreamId</code> is specified, MediaTailor returns all of the prefetch schedules with an exact match on <code>StreamId</code>. If not specified, MediaTailor returns all of the prefetch schedules for the playback configuration, regardless of <code>StreamId</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Consumption\",\n    \"Retrieval\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-create-prefetch-schedule-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreatePrefetchScheduleRequest
---
