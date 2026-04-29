---
description: Policy schema from Aqua Security API
layout: schema
name: Policy
properties_list:
- description: Policy name
  name: name
  type: string
- description: Policy description
  name: description
  type: string
- description: Whether to block containers that fail policy evaluation
  name: block_failed
  type: boolean
- description: Maximum CVSS score allowed (0-10)
  name: maximum_score
  type: number
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-policy-schema.json
slug: aqua-security-api-policy
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"default\",\n      \"description\": \"Policy name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Default security policy\",\n      \"description\": \"Policy description\"\n    },\n    \"block_failed\": {\n      \"type\": \"boolean\",\n      \"example\": true,\n      \"description\": \"Whether to block containers that fail policy evaluation\"\n    },\n    \"maximum_score\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 7.0,\n      \"description\": \"Maximum CVSS score allowed (0-10)\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-policy-schema.json\",\n  \"title\": \"Policy\",\n  \"description\": \"Policy schema from Aqua Security API\"\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-policy-schema.json
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: Policy
---
