---
description: List of statements
layout: schema
name: StatementList
properties_list:
- description: ''
  name: total_statements
  type: integer
- description: ''
  name: statements
  type: array
provider_name: Apache Livy
provider_slug: apache-livy
schema_file: json-schema/rest-api-statement-list-schema.json
slug: rest-api-statement-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-statement-list-schema.json\",\n  \"title\": \"StatementList\",\n  \"description\": \"List of statements\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total_statements\": {\n      \"type\": \"integer\",\n      \"example\": 5\n    },\n    \"statements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Statement\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-statement-list-schema.json
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: StatementList
---
