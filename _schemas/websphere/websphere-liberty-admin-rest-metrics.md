---
description: ''
layout: schema
name: Metrics
properties_list:
- description: ''
  name: scope
  type: string
- description: ''
  name: metrics
  type: object
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-admin-rest-metrics-schema.json
slug: websphere-liberty-admin-rest-metrics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Metrics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scope\": {\n      \"type\": \"string\"\n    },\n    \"metrics\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-admin-rest-metrics-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: Metrics
---
