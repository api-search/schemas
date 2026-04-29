---
description: Returns Tick History Files
layout: schema
name: TickDataLevel2
properties_list:
- description: The status of the request
  name: status
  type: string
- description: Timestamp of when request was made
  name: requestTimestamp
  type: string
- description: :"Timestamp when the file was last updated"
  name: updateTimestamp
  type: string
- description: Data Object
  name: listOfFiles
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-tick-history-tick-data-level2-schema.json
slug: factset-tick-history-tick-data-level2
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TickDataLevel2\",\n  \"type\": \"object\",\n  \"description\": \"Returns Tick History Files\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the request\"\n    },\n    \"requestTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when request was made\"\n    },\n    \"updateTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \":\\\"Timestamp when the file was last updated\\\"\"\n    },\n    \"listOfFiles\": {\n      \"type\": \"array\",\n      \"description\": \"Data Object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-tick-history-tick-data-level2-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: TickDataLevel2
---
