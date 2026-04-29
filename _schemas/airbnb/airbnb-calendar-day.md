---
description: ''
layout: schema
name: CalendarDay
properties_list:
- description: The date for this calendar entry.
  name: date
  type: string
- description: Whether the listing is available for booking on this date.
  name: available
  type: boolean
- description: The nightly price for this date in the listing currency.
  name: price
  type: number
- description: The minimum number of nights required for a stay starting on this date.
  name: minimum_nights
  type: integer
- description: The maximum number of nights allowed for a stay starting on this date.
  name: maximum_nights
  type: integer
- description: The reservation identifier if this date is booked.
  name: reservation_id
  type: string
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-calendar-day-schema.json
slug: airbnb-calendar-day
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-calendar-day-schema.json\",\n  \"title\": \"CalendarDay\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date for this calendar entry.\"\n    },\n    \"available\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the listing is available for booking on this date.\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The nightly price for this date in the listing currency.\"\n    },\n    \"minimum_nights\": {\n      \"type\": \"integer\",\n      \"description\": \"The minimum number of nights required for a stay starting on this date.\",\n      \"minimum\": 1\n    },\n    \"maximum_nights\": {\n      \"type\": \"integer\",\n\
  \      \"description\": \"The maximum number of nights allowed for a stay starting on this date.\"\n    },\n    \"reservation_id\": {\n      \"type\": \"string\",\n      \"description\": \"The reservation identifier if this date is booked.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-calendar-day-schema.json
tags: []
title: CalendarDay
---
