---
description: Object denoting that the endpoint response is possibly incomplete.
layout: schema
name: PartialOutputObject
properties_list:
- description: 'Flag indicating that the response is a possibly incomplete array or an object containing a possibly incomplete array, due to hitting a processing time limit. If `true`, some matching results might be '
  name: isPartial
  type: boolean
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-real-time-quotes-partial-output-object-schema.json
slug: factset-real-time-quotes-partial-output-object
source_filename: factset-real-time-quotes-partial-output-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PartialOutputObject\",\n  \"type\": \"object\",\n  \"description\": \"Object denoting that the endpoint response is possibly incomplete.\",\n  \"properties\": {\n    \"isPartial\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating that the response is a possibly incomplete array or an object containing a possibly incomplete array, due to hitting a processing time limit. If `true`, some matching results might be missing from the array, or elements for matching results might be incorrectly included (for example, when priority sorting would have removed the element). Depending on the use case, such a response may be unsuitable.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-real-time-quotes-partial-output-object-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: PartialOutputObject
---
