---
description: ''
layout: schema
name: PerformanceData
properties_list:
- description: Performance module name
  name: module
  type: string
- description: ''
  name: timestamp
  type: string
- description: ''
  name: metrics
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-admin-rest-performance-data-schema.json
slug: websphere-admin-rest-performance-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PerformanceData\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"module\": {\n      \"type\": \"string\",\n      \"description\": \"Performance module name\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\"\n    },\n    \"metrics\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-admin-rest-performance-data-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: PerformanceData
---
