---
description: A file parsing request for processing uploaded CSV or spreadsheet files in Torii.
layout: schema
name: Torii Parsing Request
properties_list:
- description: Unique identifier for the parsing request.
  name: id
  type: string
- description: Associated file ID.
  name: fileId
  type: string
- description: Current status of the parsing request.
  name: status
  type: string
- description: Detected columns from the file.
  name: columns
  type: array
- description: When the parsing request was created.
  name: createdAt
  type: string
provider_name: Torii
provider_slug: torii
schema_file: json-schema/parsing-request.json
slug: parsing-request
source_filename: parsing-request.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/parsing-request.json\",\n  \"title\": \"Torii Parsing Request\",\n  \"description\": \"A file parsing request for processing uploaded CSV or spreadsheet files in Torii.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the parsing request.\"\n    },\n    \"fileId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated file ID.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the parsing request.\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Detected columns from the file.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"When the parsing request was created.\"\n    }\n  },\n  \"required\": [\"id\", \"fileId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/parsing-request.json
tags:
- SaaS Management
title: Torii Parsing Request
---
