---
description: User account
layout: schema
name: User
properties_list:
- description: User identifier
  name: id
  type: string
- description: Username
  name: username
  type: string
- description: Email address
  name: email
  type: string
- description: Assigned roles
  name: roles
  type: array
- description: Whether the account is locked
  name: locked
  type: boolean
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-user-schema.json
slug: apache-shiro-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"User account\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"User identifier\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Username\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email address\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Assigned roles\"\n    },\n    \"locked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account is locked\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-user-schema.json
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: User
---
