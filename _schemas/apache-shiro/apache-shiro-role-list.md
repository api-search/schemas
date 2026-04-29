---
description: List of roles for the current user
layout: schema
name: RoleList
properties_list:
- description: Current principal
  name: principal
  type: string
- description: Assigned roles
  name: roles
  type: array
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-role-list-schema.json
slug: apache-shiro-role-list
source_filename: apache-shiro-role-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-role-list-schema.json\",\n  \"title\": \"RoleList\",\n  \"description\": \"List of roles for the current user\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"principal\": {\n      \"type\": \"string\",\n      \"description\": \"Current principal\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Assigned roles\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-role-list-schema.json
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: RoleList
---
