---
description: ''
layout: schema
name: eventRequestBody
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
- description: Comma delimited string of identifiers. An identifier can be a ticker, FactSet entity id, CUSIP or ISIN. You must provide a list of identifiers either via a ids or a portfolios parameter. If both are p
  name: ids
  type: string
- description: Name of a portfolio file stored by FactSet. If the portfolio contains more than 1,000 ids, only the first 1,000 ids are processed (e.g. client:techstocks.ofdb). Please note that using this parameter r
  name: portfolios
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
- description: Comma delimited string of sortable attributes. The sort order for each sort attribute is ascending unless it is prefixed with a minus sign, in which case it is descending.
  name: sort
  type: string
- description: The api will return resolved identifiers in the meta section of the response by default (true). If the parameter is false, the api will not attempt to resolve the identifiers.
  name: resolveIdentifiers
  type: boolean
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-signals-event-request-body-schema.json
slug: factset-signals-event-request-body
source_filename: factset-signals-event-request-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"eventRequestBody\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"A date/time (UTC) interval for filtering signal events based on their creation date. Defaults to NOW - 7 days if omitted. Users with limited access can only provide the default or a smaller date window.\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"description\": \"A date/time (UTC) interval for filtering signal events based on their last updated date. Defaults to NOW - 7 days if omitted. Users with limited access can only provide the default or a smaller date window.\"\n    },\n    \"signalIds\": {\n      \"type\": \"string\",\n      \"description\": \"Comma delimited string of signalIds\"\n    },\n    \"ids\": {\n      \"type\": \"string\",\n      \"description\": \"Comma delimited string of identifiers. An identifier can be a ticker,\
  \ FactSet entity id, CUSIP or ISIN. You must provide a list of identifiers either via a ids or a portfolios parameter. If both are provided, only ids filter is used. Users with limited access can use only the ids filter and provide at most 10 ids.\"\n    },\n    \"portfolios\": {\n      \"type\": \"string\",\n      \"description\": \"Name of a portfolio file stored by FactSet. If the portfolio contains more than 1,000 ids, only the first 1,000 ids are processed (e.g. client:techstocks.ofdb). Please note that using this parameter requires full subscription to Signals API.\"\n    },\n    \"themes\": {\n      \"type\": \"string\",\n      \"description\": \"Comma delimited string of theme ids. Full list of signal themes can be viewed at /themes.\"\n    },\n    \"categories\": {\n      \"type\": \"string\",\n      \"description\": \"Comma delimited string of category ids. Full list of signal categories can be viewed at /categories.\"\n    },\n    \"userRelevanceScore\": {\n      \"type\": \"\
  string\",\n      \"description\": \"A range for filtering signal events based on their relevancy score.\"\n    },\n    \"sort\": {\n      \"type\": \"string\",\n      \"description\": \"Comma delimited string of sortable attributes. The sort order for each sort attribute is ascending unless it is prefixed with a minus sign, in which case it is descending.\"\n    },\n    \"resolveIdentifiers\": {\n      \"type\": \"boolean\",\n      \"description\": \"The api will return resolved identifiers in the meta section of the response by default (true). If the parameter is false, the api will not attempt to resolve the identifiers.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-signals-event-request-body-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: eventRequestBody
---
