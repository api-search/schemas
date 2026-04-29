---
description: Authentication response
layout: schema
name: AuthResponse
properties_list:
- description: ''
  name: userDetails
  type: object
- description: ''
  name: authorities
  type: array
provider_name: Apache Kylin
provider_slug: apache-kylin
schema_file: json-schema/rest-api-auth-response-schema.json
slug: rest-api-auth-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-auth-response-schema.json\",\n  \"title\": \"AuthResponse\",\n  \"description\": \"Authentication response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userDetails\": {\n      \"type\": \"object\"\n    },\n    \"authorities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-kylin/refs/heads/main/json-schema/rest-api-auth-response-schema.json
tags:
- Analytics
- Big Data
- Cube
- OLAP
- Open Source
- SQL
title: AuthResponse
---
