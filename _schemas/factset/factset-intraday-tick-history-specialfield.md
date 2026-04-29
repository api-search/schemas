---
description: ''
layout: schema
name: specialfield
properties_list:
- description: '**#NF#** - Not found. The requested symbol could not be found by the service.'
  name: NF
  type: string
- description: '**#NA#** - Not Applicable. The requested field could not be found for the requested symbol. This usually means that the field is not applicable for this type of record.'
  name: NA
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-intraday-tick-history-specialfield-schema.json
slug: factset-intraday-tick-history-specialfield
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"specialfield\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NF\": {\n      \"type\": \"string\",\n      \"description\": \"**#NF#** - Not found. The requested symbol could not be found by the service.\"\n    },\n    \"NA\": {\n      \"type\": \"object\",\n      \"description\": \"**#NA#** - Not Applicable. The requested field could not be found for the requested symbol. This usually means that the field is not applicable for this type of record.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-intraday-tick-history-specialfield-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: specialfield
---
