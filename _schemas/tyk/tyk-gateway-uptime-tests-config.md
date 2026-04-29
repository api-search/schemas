---
description: ''
layout: schema
name: UptimeTestsConfig
properties_list:
- description: ''
  name: expire_utime_after
  type: integer
- description: ''
  name: recheck_wait
  type: integer
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-uptime-tests-config-schema.json
slug: tyk-gateway-uptime-tests-config
source_filename: tyk-gateway-uptime-tests-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UptimeTestsConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expire_utime_after\": {\n      \"type\": \"integer\"\n    },\n    \"recheck_wait\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-uptime-tests-config-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: UptimeTestsConfig
---
