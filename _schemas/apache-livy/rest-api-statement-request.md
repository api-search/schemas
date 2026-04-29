---
description: Request to execute a code statement
layout: schema
name: StatementRequest
properties_list:
- description: Code to execute
  name: code
  type: string
- description: Code type (defaults to session kind)
  name: kind
  type: string
provider_name: Apache Livy
provider_slug: apache-livy
schema_file: json-schema/rest-api-statement-request-schema.json
slug: rest-api-statement-request
source_filename: rest-api-statement-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-statement-request-schema.json\",\n  \"title\": \"StatementRequest\",\n  \"description\": \"Request to execute a code statement\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Code to execute\",\n      \"example\": \"1 + 1\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Code type (defaults to session kind)\",\n      \"enum\": [\n        \"spark\",\n        \"pyspark\",\n        \"sparkr\",\n        \"sql\"\n      ]\n    }\n  },\n  \"required\": [\n    \"code\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-livy/refs/heads/main/json-schema/rest-api-statement-request-schema.json
tags:
- Big Data
- Interactive Computing
- Open Source
- REST
- Spark
title: StatementRequest
---
