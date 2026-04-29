---
description: List of users
layout: schema
name: UserList
properties_list:
- description: ''
  name: users
  type: array
- description: ''
  name: total
  type: integer
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-user-list-schema.json
slug: apache-shiro-user-list
source_filename: apache-shiro-user-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-user-list-schema.json\",\n  \"title\": \"UserList\",\n  \"description\": \"List of users\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/User\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-user-list-schema.json
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: UserList
---
