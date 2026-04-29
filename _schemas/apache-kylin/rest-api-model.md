---
description: A Kylin data model
layout: schema
name: Model
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: factTable
  type: string
- description: ''
  name: status
  type: string
provider_name: Apache Kylin
provider_slug: apache-kylin
schema_file: json-schema/rest-api-model-schema.json
slug: rest-api-model
source_filename: rest-api-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-model-schema.json\",\n  \"title\": \"Model\",\n  \"description\": \"A Kylin data model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"kylin_sales_model\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Sales data model\"\n    },\n    \"factTable\": {\n      \"type\": \"string\",\n      \"example\": \"KYLIN_SALES\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"ONLINE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-model-schema.json
tags:
- Analytics
- Big Data
- Cube
- OLAP
- Open Source
- SQL
title: Model
---
