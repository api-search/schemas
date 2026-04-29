---
description: ''
layout: schema
name: eventHeadlineDataItem
properties_list:
- description: The id that was requested. This can be a ticker, cusip or factset entity id.
  name: requestId
  type: string
- description: Name of the company reported in signal. Omitted if null.
  name: companyName
  type: string
- description: Signal Id for this event. e.g. dilutionTrigger
  name: signalId
  type: string
- description: Signal Name for this event. e.g. dilutionTrigger
  name: signalName
  type: string
- description: Theme name of the signal for this event. e.g. Debt Capital Structure
  name: theme
  type: string
- description: Primary data provider for the signal this event belongs to. e.g. FactSet, Bitvore
  name: source
  type: string
- description: A unique id for this event.
  name: eventId
  type: string
- description: The UTC date/time of the event in ISO 8601 format.
  name: eventDate
  type: string
- description: One sentence summary of the event.
  name: summary
  type: string
- description: Relevancy score of this event for the requesting user on a scale of 0 to 1. Higher value indicates more relevancy.
  name: userRelevanceScore
  type: number
- description: Date/Time in UTC the event was first recorded in our data store.
  name: created
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-signals-event-headline-data-item-schema.json
slug: factset-signals-event-headline-data-item
source_filename: factset-signals-event-headline-data-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"eventHeadlineDataItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The id that was requested. This can be a ticker, cusip or factset entity id.\"\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the company reported in signal. Omitted if null.\"\n    },\n    \"signalId\": {\n      \"type\": \"string\",\n      \"description\": \"Signal Id for this event. e.g. dilutionTrigger\"\n    },\n    \"signalName\": {\n      \"type\": \"string\",\n      \"description\": \"Signal Name for this event. e.g. dilutionTrigger\"\n    },\n    \"theme\": {\n      \"type\": \"string\",\n      \"description\": \"Theme name of the signal for this event. e.g. Debt Capital Structure\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Primary data provider for the\
  \ signal this event belongs to. e.g. FactSet, Bitvore\"\n    },\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique id for this event.\"\n    },\n    \"eventDate\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC date/time of the event in ISO 8601 format.\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"One sentence summary of the event.\"\n    },\n    \"userRelevanceScore\": {\n      \"type\": \"number\",\n      \"description\": \"Relevancy score of this event for the requesting user on a scale of 0 to 1. Higher value indicates more relevancy.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"Date/Time in UTC the event was first recorded in our data store.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-signals-event-headline-data-item-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: eventHeadlineDataItem
---
