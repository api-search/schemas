---
description: Array of data objects
layout: schema
name: filesOne
properties_list:
- description: Name of the file(s) generated for the query requested
  name: fileName
  type: string
- description: Download link for the TickHistory minute bars file with requested parameters. <p>The downloaded file contains isoCode, ticker, date, time, tradeOpen, tradeHigh, tradeLow, tradeClose, tradeVolume, trad
  name: url
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-tick-history-files-one-schema.json
slug: factset-tick-history-files-one
source_filename: factset-tick-history-files-one-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"filesOne\",\n  \"type\": \"object\",\n  \"description\": \"Array of data objects\",\n  \"properties\": {\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the file(s) generated for the query requested\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Download link for the TickHistory minute bars file with requested parameters. \\n\\n <p>The downloaded file contains isoCode, ticker, date, time, tradeOpen, tradeHigh, tradeLow, tradeClose, tradeVolume, tradeNumber, and tradeVWAP</P>\\n \\n <p>This download link will expire after 12 hours.</p>\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-tick-history-files-one-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: filesOne
---
