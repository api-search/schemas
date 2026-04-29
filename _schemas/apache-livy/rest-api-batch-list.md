---
description: Paginated list of batch jobs
layout: schema
name: BatchList
properties_list:
- description: ''
  name: from
  type: integer
- description: ''
  name: total
  type: integer
- description: ''
  name: sessions
  type: array
provider_name: Apache Livy
provider_slug: apache-livy
schema_file: json-schema/rest-api-batch-list-schema.json
slug: rest-api-batch-list
source_filename: rest-api-batch-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-batch-list-schema.json\",\n  \"title\": \"BatchList\",\n  \"description\": \"Paginated list of batch jobs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 3\n    },\n    \"sessions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Batch\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-batch-list-schema.json
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: BatchList
---
