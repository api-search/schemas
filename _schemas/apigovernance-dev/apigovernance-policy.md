---
description: An API governance policy composed of multiple guidelines.
layout: schema
name: Policy
properties_list:
- description: Policy identifier.
  name: id
  type: string
- description: Policy name.
  name: name
  type: string
- description: Policy description.
  name: description
  type: string
- description: List of guideline IDs included in this policy.
  name: guidelines
  type: array
- description: How this policy is enforced.
  name: enforcement
  type: string
provider_name: APIGovernance.Dev
provider_slug: apigovernance-dev
schema_file: json-schema/apigovernance-policy-schema.json
slug: apigovernance-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apigovernance-dev/refs/heads/main/json-schema/apigovernance-policy-schema.json\",\n  \"title\": \"Policy\",\n  \"description\": \"An API governance policy composed of multiple guidelines.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Policy identifier.\",\n      \"example\": \"pol-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Policy name.\",\n      \"example\": \"API Security Policy\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Policy description.\"\n    },\n    \"guidelines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of guideline IDs included in this policy.\"\n    },\n    \"enforcement\": {\n      \"type\": \"string\"\
  ,\n      \"enum\": [\n        \"blocking\",\n        \"advisory\",\n        \"informational\"\n      ],\n      \"description\": \"How this policy is enforced.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apigovernance-dev/refs/heads/main/json-schema/apigovernance-policy-schema.json
tags:
- API Design
- API Governance
- Best Practices
- Compliance
- Guidelines
- Standards
title: Policy
---
