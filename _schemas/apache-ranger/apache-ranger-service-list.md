---
description: List of Ranger services
layout: schema
name: ServiceList
properties_list:
- description: ''
  name: totalCount
  type: integer
- description: ''
  name: services
  type: array
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-service-list-schema.json
slug: apache-ranger-service-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-service-list-schema.json\",\n  \"title\": \"ServiceList\",\n  \"description\": \"List of Ranger services\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\"\n    },\n    \"services\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RangerService\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-service-list-schema.json
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: ServiceList
---
