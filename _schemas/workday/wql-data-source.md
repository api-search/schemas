---
description: ''
layout: schema
name: DataSource
properties_list:
- description: The Workday ID of the data source.
  name: id
  type: string
- description: A display descriptor for the data source.
  name: descriptor
  type: string
- description: The name of the data source used in WQL FROM clauses.
  name: name
  type: string
- description: The plural name of the data source.
  name: pluralName
  type: string
- description: The fields available in this data source.
  name: fields
  type: array
provider_name: Workday
provider_slug: workday
schema_file: json-schema/wql-data-source-schema.json
slug: wql-data-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the data source.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the data source.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the data source used in WQL FROM clauses.\"\n    },\n    \"pluralName\": {\n      \"type\": \"string\",\n      \"description\": \"The plural name of the data source.\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"The fields available in this data source.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/wql-data-source-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: DataSource
---
