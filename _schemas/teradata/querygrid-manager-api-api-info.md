---
description: QueryGrid Manager API information.
layout: schema
name: ApiInfo
properties_list:
- description: API version number.
  name: version
  type: string
- description: Build version string.
  name: build
  type: string
- description: Current API status.
  name: status
  type: string
provider_name: Teradata
provider_slug: teradata
schema_file: json-schema/querygrid-manager-api-api-info-schema.json
slug: querygrid-manager-api-api-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-api-info-schema.json\",\n  \"title\": \"ApiInfo\",\n  \"description\": \"QueryGrid Manager API information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"API version number.\"\n    },\n    \"build\": {\n      \"type\": \"string\",\n      \"description\": \"Build version string.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current API status.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-api-info-schema.json
tags:
- Analytics
- Cloud
- Data Management
- Data Warehousing
- Database
- Enterprise
- Machine Learning
- SQL
title: ApiInfo
---
