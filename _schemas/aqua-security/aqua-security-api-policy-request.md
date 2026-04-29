---
description: PolicyRequest schema from Aqua Security API
layout: schema
name: PolicyRequest
properties_list:
- description: Policy name (unique)
  name: name
  type: string
- description: Policy description
  name: description
  type: string
- description: Block containers failing policy
  name: block_failed
  type: boolean
- description: Maximum CVSS score threshold
  name: maximum_score
  type: number
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-policy-request-schema.json
slug: aqua-security-api-policy-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"high-security\",\n      \"description\": \"Policy name (unique)\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Policy blocking high severity vulnerabilities\",\n      \"description\": \"Policy description\"\n    },\n    \"block_failed\": {\n      \"type\": \"boolean\",\n      \"example\": true,\n      \"description\": \"Block containers failing policy\"\n    },\n    \"maximum_score\": {\n      \"type\": \"number\",\n      \"example\": 7.0,\n      \"description\": \"Maximum CVSS score threshold\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-policy-request-schema.json\",\n  \"title\": \"PolicyRequest\",\n  \"description\": \"PolicyRequest\
  \ schema from Aqua Security API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-policy-request-schema.json
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: PolicyRequest
---
