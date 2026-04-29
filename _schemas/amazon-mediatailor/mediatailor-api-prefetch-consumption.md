---
description: A complex type that contains settings that determine how and when that MediaTailor places prefetched ads into upcoming ad breaks.
layout: schema
name: PrefetchConsumption
properties_list:
- description: ''
  name: AvailMatchingCriteria
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: StartTime
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-prefetch-consumption-schema.json
slug: mediatailor-api-prefetch-consumption
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-prefetch-consumption-schema.json\",\n  \"title\": \"PrefetchConsumption\",\n  \"description\": \"A complex type that contains settings that determine how and when that MediaTailor places prefetched ads into upcoming ad breaks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailMatchingCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAvailMatchingCriteria\"\n        },\n        {\n          \"description\": \"If you only want MediaTailor to insert prefetched ads into avails (ad breaks) that match specific dynamic variables, such as <code>scte.event_id</code>, set the avail matching criteria.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\
  \n        },\n        {\n          \"description\": \"The time when MediaTailor no longer considers the prefetched ads for use in an ad break. MediaTailor automatically deletes prefetch schedules no less than seven days after the end time. If you'd like to manually delete the prefetch schedule, you can call <code>DeletePrefetchSchedule</code>.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"description\": \"The time when prefetched ads are considered for use in an ad break. If you don't specify <code>StartTime</code>, the prefetched ads are available after MediaTailor retrives them from the ad decision server.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-prefetch-consumption-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PrefetchConsumption
---
