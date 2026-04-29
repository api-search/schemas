---
description: A data center configuration.
layout: schema
name: DataCenter
properties_list:
- description: Unique data center identifier.
  name: id
  type: string
- description: Data center name.
  name: name
  type: string
- description: Data center description.
  name: description
  type: string
- description: Physical location.
  name: location
  type: string
provider_name: Teradata
provider_slug: teradata
schema_file: json-schema/querygrid-manager-api-data-center-schema.json
slug: querygrid-manager-api-data-center
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-data-center-schema.json\",\n  \"title\": \"DataCenter\",\n  \"description\": \"A data center configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique data center identifier.\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Data center name.\" },\n    \"description\": { \"type\": \"string\", \"description\": \"Data center description.\" },\n    \"location\": { \"type\": \"string\", \"description\": \"Physical location.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-data-center-schema.json
tags:
- Analytics
- Cloud
- Data Management
- Data Warehousing
- Database
- Enterprise
- Machine Learning
- SQL
title: DataCenter
---
