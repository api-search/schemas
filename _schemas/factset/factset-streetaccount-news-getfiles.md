---
description: ''
layout: schema
name: getfiles
properties_list:
- description: Defines the name of the product
  name: product
  type: string
- description: The startDate from which the data is required in YYYY-MM-DDTHH:MM:SSZ format
  name: startDate
  type: string
- description: The endDate until which the data is fetched in YYYY-MM-DDTHH:MM:SSZ format
  name: endDate
  type: string
- description: Unique id to get the xml files for the requested date
  name: jobID
  type: string
- description: Defines the status of the request
  name: status
  type: string
- description: Link to download the zip file which contains xml files
  name: url
  type: string
- description: Returns the part number of the jobID
  name: part
  type: integer
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-streetaccount-news-getfiles-schema.json
slug: factset-streetaccount-news-getfiles
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"getfiles\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"product\": {\n      \"type\": \"string\",\n      \"description\": \"Defines the name of the product\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"The startDate from which the data is required in YYYY-MM-DDTHH:MM:SSZ format\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"The endDate until which the data is fetched in YYYY-MM-DDTHH:MM:SSZ format\"\n    },\n    \"jobID\": {\n      \"type\": \"string\",\n      \"description\": \"Unique id to get the xml files for the requested date\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Defines the status of the request\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Link to download the zip file which contains xml files\"\n    },\n    \"part\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Returns the part number of the jobID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-streetaccount-news-getfiles-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: getfiles
---
