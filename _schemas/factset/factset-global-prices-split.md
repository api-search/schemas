---
description: ''
layout: schema
name: Split
properties_list:
- description: Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equit
  name: fsymId
  type: string
- description: FactSet identifier that uniquely identifies the Event.
  name: eventId
  type: string
- description: Character code that denotes the type of Event.
  name: eventTypeCode
  type: string
- description: Corporate Actions Event type description.
  name: eventTypeDesc
  type: string
- description: Date Event was announced in YYYY-MM-DD format.
  name: announcementDate
  type: string
- description: Date of Record for distribution in YYYY-MM-DD format.
  name: recordDate
  type: string
- description: Date of Payment for distribution in YYYY-MM-DD format.
  name: payDate
  type: string
- description: Effective Date or Ex-Date of distribution in YYYY-MM-DD format.
  name: effectiveDate
  type: string
- description: Factor for adjusting price and shares. A 2-for-1 split returns .50, the number you would multiply the stock price by to adjust for the split.
  name: adjFactor
  type: number
- description: Combined adjustment factor for all distribution events on that day.
  name: adjFactorCombined
  type: number
- description: Component of distribution ratio - Number of shares held.
  name: distOldTerm
  type: number
- description: Component of distribution ratio - Number of shares received.
  name: distNewTerm
  type: number
- description: Parent Spin-Off for a company
  name: distInstFsymId
  type: string
- description: Textual description identifying the event.
  name: shortDesc
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-global-prices-split-schema.json
slug: factset-global-prices-split
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Split\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equities, all primary listings per region and currency are allocated a regional-level permanent identifier. The regional-level permanent identifier will be available once a SEDOL representing the region/currency has been allocated and the identifiers are on FactSet.\"\n    },\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet identifier that uniquely identifies the Event.\"\n    },\n    \"eventTypeCode\": {\n      \"type\": \"string\",\n      \"description\": \"Character code that denotes the type of Event.\"\n    },\n    \"eventTypeDesc\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Corporate Actions Event type description.\"\n    },\n    \"announcementDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date Event was announced in YYYY-MM-DD format.\"\n    },\n    \"recordDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of Record for distribution in YYYY-MM-DD format.\"\n    },\n    \"payDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of Payment for distribution in YYYY-MM-DD format.\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"description\": \"Effective Date or Ex-Date of distribution in YYYY-MM-DD format.\"\n    },\n    \"adjFactor\": {\n      \"type\": \"number\",\n      \"description\": \"Factor for adjusting price and shares.\\nA 2-for-1 split returns .50, the number you would multiply the stock price by to adjust for the split.\\n\"\n    },\n    \"adjFactorCombined\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Combined adjustment factor for all distribution events on that day.\"\n    },\n    \"distOldTerm\": {\n      \"type\": \"number\",\n      \"description\": \"Component of distribution ratio -  Number of shares held.\"\n    },\n    \"distNewTerm\": {\n      \"type\": \"number\",\n      \"description\": \"Component of distribution ratio -  Number of shares received.\"\n    },\n    \"distInstFsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent Spin-Off for a company\"\n    },\n    \"shortDesc\": {\n      \"type\": \"string\",\n      \"description\": \"Textual description identifying the event.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-global-prices-split-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Split
---
