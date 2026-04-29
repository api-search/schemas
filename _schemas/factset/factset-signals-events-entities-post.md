---
description: ''
layout: schema
name: eventsEntitiesPost
properties_list:
- description: A date/time (UTC) interval for filtering signal events based on their creation date. Defaults to NOW - 7 days if omitted. Users with limited access can only provide the default or a smaller date windo
  name: created
  type: string
- description: A date/time (UTC) interval for filtering signal events based on their last updated date. Defaults to NOW - 7 days if omitted. Users with limited access can only provide the default or a smaller date w
  name: updated
  type: string
- description: Comma delimited string of signalIds
  name: signalIds
  type: string
- description: Comma delimited string of theme ids. Full list of signal themes can be viewed at /themes.
  name: themes
  type: string
- description: Comma delimited string of category ids. Full list of signal categories can be viewed at /categories.
  name: categories
  type: string
- description: A range for filtering signal events based on their relevancy score.
  name: userRelevanceScore
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-signals-events-entities-post-schema.json
slug: factset-signals-events-entities-post
source_filename: factset-signals-events-entities-post-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"eventsEntitiesPost\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"A date/time (UTC) interval for filtering signal events based on their creation date. Defaults to NOW - 7 days if omitted. Users with limited access can only provide the default or a smaller date window.\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"description\": \"A date/time (UTC) interval for filtering signal events based on their last updated date. Defaults to NOW - 7 days if omitted. Users with limited access can only provide the default or a smaller date window.\"\n    },\n    \"signalIds\": {\n      \"type\": \"string\",\n      \"description\": \"Comma delimited string of signalIds\"\n    },\n    \"themes\": {\n      \"type\": \"string\",\n      \"description\": \"Comma delimited string of theme ids. Full list of signal themes\
  \ can be viewed at /themes.\"\n    },\n    \"categories\": {\n      \"type\": \"string\",\n      \"description\": \"Comma delimited string of category ids. Full list of signal categories can be viewed at /categories.\"\n    },\n    \"userRelevanceScore\": {\n      \"type\": \"string\",\n      \"description\": \"A range for filtering signal events based on their relevancy score.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-signals-events-entities-post-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: eventsEntitiesPost
---
