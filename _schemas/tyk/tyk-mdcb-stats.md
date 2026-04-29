---
description: ''
layout: schema
name: Stats
properties_list:
- description: ''
  name: apis_count
  type: integer
- description: ''
  name: policies_count
  type: integer
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-mdcb-stats-schema.json
slug: tyk-mdcb-stats
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Stats\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apis_count\": {\n      \"type\": \"integer\"\n    },\n    \"policies_count\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-mdcb-stats-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: Stats
---
