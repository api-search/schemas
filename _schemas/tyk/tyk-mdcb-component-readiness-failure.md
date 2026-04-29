---
description: ''
layout: schema
name: ComponentReadinessFailure
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: observation_ts
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-mdcb-component-readiness-failure-schema.json
slug: tyk-mdcb-component-readiness-failure
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ComponentReadinessFailure\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"observation_ts\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-mdcb-component-readiness-failure-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: ComponentReadinessFailure
---
