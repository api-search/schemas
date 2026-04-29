---
description: GetPrefetchScheduleResponse schema from Amazon MediaTailor API
layout: schema
name: GetPrefetchScheduleResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Consumption
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: PlaybackConfigurationName
  type: object
- description: ''
  name: Retrieval
  type: object
- description: ''
  name: StreamId
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-get-prefetch-schedule-response-schema.json
slug: mediatailor-api-get-prefetch-schedule-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-get-prefetch-schedule-response-schema.json\",\n  \"title\": \"GetPrefetchScheduleResponse\",\n  \"description\": \"GetPrefetchScheduleResponse schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the prefetch schedule.\"\n        }\n      ]\n    },\n    \"Consumption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrefetchConsumption\"\n        },\n        {\n          \"description\": \"Consumption settings determine how, and when, MediaTailor places the prefetched ads into ad breaks. Ad consumption occurs within a span of time that you\
  \ define, called a <i>consumption window</i>. You can designate which ad breaks that MediaTailor fills with prefetch ads by setting avail matching criteria.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the prefetch schedule. The name must be unique among all prefetch schedules that are associated with the specified playback configuration.\"\n        }\n      ]\n    },\n    \"PlaybackConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the playback configuration to create the prefetch schedule for.\"\n        }\n      ]\n    },\n    \"Retrieval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrefetchRetrieval\"\n        },\n        {\n          \"description\": \"A complex type that contains\
  \ settings for prefetch retrieval from the ad decision server (ADS).\"\n        }\n      ]\n    },\n    \"StreamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"An optional stream identifier that you can specify in order to prefetch for multiple streams that use the same playback configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-get-prefetch-schedule-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: GetPrefetchScheduleResponse
---
