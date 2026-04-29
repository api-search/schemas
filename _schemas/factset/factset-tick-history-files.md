---
description: Array of data objects
layout: schema
name: files
properties_list:
- description: Name of the file(s) generated for the query requested
  name: fileName
  type: string
- description: Download link for the TickHistory file with requested parameters <p>This download link will expire after 24 hours</p>
  name: url
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-tick-history-files-schema.json
slug: factset-tick-history-files
source_filename: factset-tick-history-files-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"files\",\n  \"type\": \"object\",\n  \"description\": \"Array of data objects\",\n  \"properties\": {\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the file(s) generated for the query requested\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"\\nDownload link for the TickHistory file with requested parameters\\n<p>This download link will expire after 24 hours</p>\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-tick-history-files-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: files
---
