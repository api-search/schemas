---
description: ''
layout: schema
name: requestfilesResponse
properties_list:
- description: Unique id to get the xml files for the requested date
  name: jobID
  type: string
- description: Returns the value as submitted. Tells the request has been submitted
  name: status
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-streetaccount-news-requestfiles-response-schema.json
slug: factset-streetaccount-news-requestfiles-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"requestfilesResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobID\": {\n      \"type\": \"string\",\n      \"description\": \"Unique id to get the xml files for the requested date\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Returns the value as submitted. Tells the request has been submitted\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-streetaccount-news-requestfiles-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: requestfilesResponse
---
