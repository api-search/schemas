---
description: ''
layout: schema
name: ActivitySearchOptions
properties_list:
- description: The creation date or creation date range of the activity
  name: creationDate
  type: object
- description: The end date pf the activity (copy of the date associated to the SUCCEEDED or FAILED stage)
  name: endDate
  type: string
- description: Number of requested items per page
  name: itemsPerPage
  type: number
- description: The copy of the origin user request. It could be the whole object or only some elements.
  name: payload
  type: object
- description: A progress indicator between 0 and 100
  name: progress
  type: number
- description: Unbounded list or parameters to sort by. The '+' indicates ascendant ordering, the '-' indicates descendant ordering. If not precised, default to '+'
  name: sortBy
  type: string
- description: The start date of the activity (date of the first stage that is not QUEUED)
  name: startDate
  type: string
- description: The index of the first item present in the response
  name: startIndex
  type: number
- description: The status or status list (comma separated list) of the activity.
  name: status
  type: string
- description: Type of activity
  name: type
  type: string
- description: ''
  name: userId
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-activity-search-options-schema.json
slug: oneatlas-activity-search-options
source_filename: oneatlas-activity-search-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-activity-search-options-schema.json\",\n  \"title\": \"ActivitySearchOptions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creationDate\": {\n      \"description\": \"The creation date or creation date range of the activity\",\n      \"oneOf\": [\n        {\n          \"description\": \"The creation date of the activity.\",\n          \"example\": \"2017-08-29T00:00:00Z\",\n          \"format\": \"date-time\",\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The creation dates range.\\n\\nRanges are expressed as follow:\\n  - Comma to separate start value from end value\\n  - Start value or end value can be omitted (it means values are infinite)\\n  - Start with `[` means *start value is included*\\n  - Start with `]` means *start value is excluded*\\\
  n  - End with `[` means *end value is included*\\n  - End with `]` means *end value is excluded*\",\n          \"example\": \"[2017-08-29T00:00:00Z\",\n          \"format\": \"date-time-range\",\n          \"type\": \"string\"\n        }\n      ]\n    },\n    \"endDate\": {\n      \"description\": \"The end date pf the activity (copy of the date associated to the SUCCEEDED or FAILED stage)\",\n      \"format\": \"datetime\",\n      \"oneOf\": [\n        {\n          \"description\": \"The end date of the activity.\",\n          \"example\": \"2017-08-29T00:00:00Z\",\n          \"format\": \"date-time\",\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The end dates range.\\n\\nRanges are expressed as follow:\\n  - Comma to separate start value from end value\\n  - Start value or end value can be omitted (it means values are infinite)\\n  - Start with `[` means *start value is included*\\n  - Start with `]` means *start value is excluded*\\n  - End with\
  \ `[` means *end value is included*\\n  - End with `]` means *end value is excluded*\",\n          \"example\": \"[2017-08-29T00:00:00Z\",\n          \"format\": \"date-time-range\",\n          \"type\": \"string\"\n        }\n      ],\n      \"type\": \"string\"\n    },\n    \"itemsPerPage\": {\n      \"description\": \"Number of requested items per page\",\n      \"example\": 50,\n      \"format\": \"integer\",\n      \"minimum\": 1,\n      \"type\": \"number\"\n    },\n    \"payload\": {\n      \"description\": \"The copy of the origin user request. It could be the whole object or only some elements.\",\n      \"oneOf\": [\n        {\n          \"description\": \"The json object.\",\n          \"example\": [\n            {\n              \"workspace\": \"public\"\n            }\n          ],\n          \"type\": \"object\"\n        },\n        {\n          \"description\": \"String representation of the json object.\",\n          \"example\": \"{\\\"workspace\\\":\\\"public\\\"}\",\n\
  \          \"type\": \"string\"\n        }\n      ]\n    },\n    \"progress\": {\n      \"description\": \"A progress indicator between 0 and 100\",\n      \"format\": \"integer\",\n      \"maximum\": 100,\n      \"minimum\": 0,\n      \"type\": \"number\"\n    },\n    \"sortBy\": {\n      \"description\": \"Unbounded list or parameters to sort by. The '+' indicates ascendant ordering, the '-' indicates descendant ordering. If not precised, default to '+'\",\n      \"example\": \"+startDate,-endDate\",\n      \"type\": \"string\"\n    },\n    \"startDate\": {\n      \"description\": \"The start date of the activity (date of the first stage that is not QUEUED)\",\n      \"format\": \"datetime\",\n      \"oneOf\": [\n        {\n          \"description\": \"The start date of the activity.\",\n          \"example\": \"2017-08-29T00:00:00Z\",\n          \"format\": \"date-time\",\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The start dates range.\\n\\\
  nRanges are expressed as follow:\\n  - Comma to separate start value from end value\\n  - Start value or end value can be omitted (it means values are infinite)\\n  - Start with `[` means *start value is included*\\n  - Start with `]` means *start value is excluded*\\n  - End with `[` means *end value is included*\\n  - End with `]` means *end value is excluded*\",\n          \"example\": \"[2017-08-29T00:00:00Z\",\n          \"format\": \"date-time-range\",\n          \"type\": \"string\"\n        }\n      ],\n      \"type\": \"string\"\n    },\n    \"startIndex\": {\n      \"description\": \"The index of the first item present in the response\",\n      \"example\": 1,\n      \"format\": \"integer\",\n      \"minimum\": 0,\n      \"type\": \"number\"\n    },\n    \"status\": {\n      \"description\": \"The status or status list (comma separated list) of the activity.\",\n      \"enum\": [\n        \"QUEUED\",\n        \"RUNNING\",\n        \"ON_HOLD\",\n        \"CANCELED\",\n       \
  \ \"WAITING_CANCEL\",\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"ARCHIVED\"\n      ],\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type of activity\",\n      \"enum\": [\n        \"ingestion\",\n        \"processing\",\n        \"formatting\",\n        \"delivering\"\n      ],\n      \"type\": \"string\"\n    },\n    \"userId\": {\n      \"$ref\": \"#/components/schemas/Id\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-activity-search-options-schema.json
tags:
- Imagery
- Satellites
title: ActivitySearchOptions
---
