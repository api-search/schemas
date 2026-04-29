---
description: Log output
layout: schema
name: Log
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: from
  type: integer
- description: ''
  name: size
  type: integer
- description: ''
  name: log
  type: array
provider_name: Apache Livy
provider_slug: apache-livy
schema_file: json-schema/rest-api-log-schema.json
slug: rest-api-log
source_filename: rest-api-log-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-log-schema.json\",\n  \"title\": \"Log\",\n  \"description\": \"Log output\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"from\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"log\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-log-schema.json
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: Log
---
