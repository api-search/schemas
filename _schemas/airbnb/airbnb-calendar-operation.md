---
description: ''
layout: schema
name: CalendarOperation
properties_list:
- description: The start date of the range to update.
  name: start_date
  type: string
- description: The end date of the range to update.
  name: end_date
  type: string
- description: Whether the dates should be available or blocked.
  name: available
  type: boolean
- description: The nightly price to set for this date range.
  name: price
  type: number
- description: The minimum number of nights required for stays in this range.
  name: minimum_nights
  type: integer
- description: The maximum number of nights allowed for stays in this range.
  name: maximum_nights
  type: integer
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-calendar-operation-schema.json
slug: airbnb-calendar-operation
source_filename: airbnb-calendar-operation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-calendar-operation-schema.json\",\n  \"title\": \"CalendarOperation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The start date of the range to update.\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The end date of the range to update.\"\n    },\n    \"available\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the dates should be available or blocked.\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The nightly price to set for this date range.\",\n      \"minimum\": 0\n    },\n    \"minimum_nights\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"The minimum number of nights required for stays in this range.\",\n      \"minimum\": 1\n    },\n    \"maximum_nights\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of nights allowed for stays in this range.\"\n    }\n  },\n  \"required\": [\n    \"start_date\",\n    \"end_date\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-calendar-operation-schema.json
tags: []
title: CalendarOperation
---
