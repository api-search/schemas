---
description: Permission check request
layout: schema
name: PermissionCheckRequest
properties_list:
- description: Shiro permission string (e.g. printer:print, user:edit:123)
  name: permission
  type: string
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-permission-check-request-schema.json
slug: apache-shiro-permission-check-request
source_filename: apache-shiro-permission-check-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-permission-check-request-schema.json\",\n  \"title\": \"PermissionCheckRequest\",\n  \"description\": \"Permission check request\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permission\": {\n      \"type\": \"string\",\n      \"description\": \"Shiro permission string (e.g. printer:print, user:edit:123)\"\n    }\n  },\n  \"required\": [\n    \"permission\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-shiro/refs/heads/main/json-schema/apache-shiro-permission-check-request-schema.json
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: PermissionCheckRequest
---
