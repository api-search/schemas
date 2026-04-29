---
description: ''
layout: schema
name: checkstatus
properties_list:
- description: Defines the name of the product
  name: product
  type: string
- description: Unique id to get the xml files for the requested date
  name: jobID
  type: string
- description: Returns any of the 2 results Submitted ->Running->Completed and Failed
  name: status
  type: string
- description: Returns how much percentage of task is completed for the requested jobID
  name: percentDone
  type: integer
- description: The date from which the data is required in YYYY-MM-DDTHH:MM:SSZ format
  name: startDate
  type: string
- description: The date until which the data is fetched in YYYY-MM-DDTHH:MM:SSZ format
  name: endDate
  type: string
- description: Returns the part number of the jobID
  name: part
  type: integer
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-streetaccount-news-checkstatus-schema.json
slug: factset-streetaccount-news-checkstatus
source_filename: factset-streetaccount-news-checkstatus-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"checkstatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"product\": {\n      \"type\": \"string\",\n      \"description\": \"Defines the name of the product\"\n    },\n    \"jobID\": {\n      \"type\": \"string\",\n      \"description\": \"Unique id to get the xml files for the requested date\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Returns any of the 2 results Submitted ->Running->Completed and Failed\"\n    },\n    \"percentDone\": {\n      \"type\": \"integer\",\n      \"description\": \"Returns how much percentage of  task is completed for the requested jobID\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date from which the data is required in YYYY-MM-DDTHH:MM:SSZ format\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date until which the data is fetched\
  \ in YYYY-MM-DDTHH:MM:SSZ format\"\n    },\n    \"part\": {\n      \"type\": \"integer\",\n      \"description\": \"Returns the part number of the jobID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-streetaccount-news-checkstatus-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: checkstatus
---
