---
description: User login credentials
layout: schema
name: LoginRequest
properties_list:
- description: Username or email
  name: username
  type: string
- description: User password
  name: password
  type: string
- description: Whether to set remember-me cookie
  name: rememberMe
  type: boolean
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-login-request-schema.json
slug: apache-shiro-login-request
source_filename: apache-shiro-login-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-login-request-schema.json\",\n  \"title\": \"LoginRequest\",\n  \"description\": \"User login credentials\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Username or email\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"User password\"\n    },\n    \"rememberMe\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to set remember-me cookie\"\n    }\n  },\n  \"required\": [\n    \"username\",\n    \"password\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-login-request-schema.json
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: LoginRequest
---
