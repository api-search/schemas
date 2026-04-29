---
description: Knox gateway version information
layout: schema
name: KnoxVersion
properties_list:
- description: Knox version string
  name: version
  type: string
- description: Build hash
  name: hash
  type: string
provider_name: Apache Knox
provider_slug: apache-knox
schema_file: json-schema/admin-api-knox-version-schema.json
slug: admin-api-knox-version
source_filename: admin-api-knox-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-knox/refs/heads/main/json-schema/admin-api-knox-version-schema.json\",\n  \"title\": \"KnoxVersion\",\n  \"description\": \"Knox gateway version information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Knox version string\",\n      \"example\": \"2.0.0\"\n    },\n    \"hash\": {\n      \"type\": \"string\",\n      \"description\": \"Build hash\",\n      \"example\": \"abc123def\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-knox/refs/heads/main/json-schema/admin-api-knox-version-schema.json
tags:
- API Gateway
- Authentication
- Hadoop
- Open Source
- Security
- SSO
title: KnoxVersion
---
