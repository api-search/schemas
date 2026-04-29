---
description: Successful authentication response
layout: schema
name: LoginResponse
properties_list:
- description: Shiro session identifier
  name: sessionId
  type: string
- description: Authenticated principal name
  name: principal
  type: string
- description: Roles assigned to the user
  name: roles
  type: array
- description: Explicit permissions granted to the user
  name: permissions
  type: array
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-login-response-schema.json
slug: apache-shiro-login-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-login-response-schema.json\",\n  \"title\": \"LoginResponse\",\n  \"description\": \"Successful authentication response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"description\": \"Shiro session identifier\"\n    },\n    \"principal\": {\n      \"type\": \"string\",\n      \"description\": \"Authenticated principal name\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Roles assigned to the user\"\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Explicit permissions granted to the user\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-login-response-schema.json
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: LoginResponse
---
