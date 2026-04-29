---
description: List of available Data Cloud connections
layout: schema
name: ConnectionList
properties_list:
- description: ''
  name: connections
  type: array
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-data-cloud-connection-list-schema.json
slug: aladdin-studio-data-cloud-connection-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-data-cloud-connection-list-schema.json\",\n  \"title\": \"ConnectionList\",\n  \"description\": \"List of available Data Cloud connections\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connections\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Connection\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-data-cloud-connection-list-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: ConnectionList
---
