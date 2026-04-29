---
description: List of Ranger security policies
layout: schema
name: PolicyList
properties_list:
- description: Total number of policies
  name: totalCount
  type: integer
- description: ''
  name: pageSize
  type: integer
- description: ''
  name: resultSize
  type: integer
- description: ''
  name: policies
  type: array
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-policy-list-schema.json
slug: apache-ranger-policy-list
source_filename: apache-ranger-policy-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-policy-list-schema.json\",\n  \"title\": \"PolicyList\",\n  \"description\": \"List of Ranger security policies\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of policies\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\"\n    },\n    \"resultSize\": {\n      \"type\": \"integer\"\n    },\n    \"policies\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Policy\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-policy-list-schema.json
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: PolicyList
---
