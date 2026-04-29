---
description: JWT or token-based authentication response
layout: schema
name: TokenResponse
properties_list:
- description: Authentication token
  name: token
  type: string
- description: Token type (e.g. Bearer)
  name: tokenType
  type: string
- description: Token expiry in seconds
  name: expiresIn
  type: integer
- description: Authenticated principal
  name: principal
  type: string
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-token-response-schema.json
slug: apache-shiro-token-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-token-response-schema.json\",\n  \"title\": \"TokenResponse\",\n  \"description\": \"JWT or token-based authentication response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication token\"\n    },\n    \"tokenType\": {\n      \"type\": \"string\",\n      \"description\": \"Token type (e.g. Bearer)\"\n    },\n    \"expiresIn\": {\n      \"type\": \"integer\",\n      \"description\": \"Token expiry in seconds\"\n    },\n    \"principal\": {\n      \"type\": \"string\",\n      \"description\": \"Authenticated principal\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-token-response-schema.json
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: TokenResponse
---
