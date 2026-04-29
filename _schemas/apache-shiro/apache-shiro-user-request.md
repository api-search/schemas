---
description: Request to create a user
layout: schema
name: UserRequest
properties_list:
- description: ''
  name: username
  type: string
- description: ''
  name: password
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: roles
  type: array
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-user-request-schema.json
slug: apache-shiro-user-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-user-request-schema.json\",\n  \"title\": \"UserRequest\",\n  \"description\": \"Request to create a user\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\"\n    },\n    \"password\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"username\",\n    \"password\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-user-request-schema.json
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: UserRequest
---
