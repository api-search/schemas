---
description: Result of permission check
layout: schema
name: PermissionCheckResult
properties_list:
- description: Checked permission string
  name: permission
  type: string
- description: Whether the subject has the permission
  name: permitted
  type: boolean
- description: Subject being checked
  name: principal
  type: string
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-permission-check-result-schema.json
slug: apache-shiro-permission-check-result
source_filename: apache-shiro-permission-check-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-permission-check-result-schema.json\",\n  \"title\": \"PermissionCheckResult\",\n  \"description\": \"Result of permission check\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permission\": {\n      \"type\": \"string\",\n      \"description\": \"Checked permission string\"\n    },\n    \"permitted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the subject has the permission\"\n    },\n    \"principal\": {\n      \"type\": \"string\",\n      \"description\": \"Subject being checked\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-permission-check-result-schema.json
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: PermissionCheckResult
---
