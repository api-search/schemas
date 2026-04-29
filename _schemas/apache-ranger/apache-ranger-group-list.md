---
description: List of Ranger groups
layout: schema
name: GroupList
properties_list:
- description: ''
  name: totalCount
  type: integer
- description: ''
  name: groups
  type: array
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-group-list-schema.json
slug: apache-ranger-group-list
source_filename: apache-ranger-group-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-group-list-schema.json\",\n  \"title\": \"GroupList\",\n  \"description\": \"List of Ranger groups\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RangerGroup\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-group-list-schema.json
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: GroupList
---
