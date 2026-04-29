---
description: Date-Time
layout: schema
name: dateTimePeriodMin
properties_list:
- description: The date for (or from which) the data is required. Supports in YYYY-MM-DDTHH:MM:SSZ format.
  name: start
  type: string
- description: The date to which data is required. Supports in YYYY-MM-DDTHH:MM:SSZ format.
  name: end
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-tick-history-date-time-period-min-schema.json
slug: factset-tick-history-date-time-period-min
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"dateTimePeriodMin\",\n  \"type\": \"object\",\n  \"description\": \"Date-Time\\n\",\n  \"properties\": {\n    \"start\": {\n      \"type\": \"string\",\n      \"description\": \"The date for (or from which) the data is required. Supports in YYYY-MM-DDTHH:MM:SSZ format.\\n\"\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"description\": \"The date to which data is required. Supports in YYYY-MM-DDTHH:MM:SSZ format.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-tick-history-date-time-period-min-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: dateTimePeriodMin
---
