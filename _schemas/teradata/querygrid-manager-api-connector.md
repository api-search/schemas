---
description: A connector for system integration.
layout: schema
name: Connector
properties_list:
- description: Unique connector identifier.
  name: id
  type: string
- description: Connector name.
  name: name
  type: string
- description: Connector type.
  name: type
  type: string
- description: Connector version.
  name: version
  type: string
- description: Connector status.
  name: status
  type: string
provider_name: Teradata
provider_slug: teradata
schema_file: json-schema/querygrid-manager-api-connector-schema.json
slug: querygrid-manager-api-connector
source_filename: querygrid-manager-api-connector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-connector-schema.json\",\n  \"title\": \"Connector\",\n  \"description\": \"A connector for system integration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique connector identifier.\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Connector name.\" },\n    \"type\": { \"type\": \"string\", \"description\": \"Connector type.\" },\n    \"version\": { \"type\": \"string\", \"description\": \"Connector version.\" },\n    \"status\": { \"type\": \"string\", \"description\": \"Connector status.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-connector-schema.json
tags:
- Analytics
- Cloud
- Data Management
- Data Warehousing
- Database
- Enterprise
- Machine Learning
- SQL
title: Connector
---
