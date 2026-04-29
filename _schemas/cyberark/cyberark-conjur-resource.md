---
description: A managed object in Conjur policy (user, host, group, layer, variable, policy, or webservice).
layout: schema
name: ConjurResource
properties_list:
- description: Fully qualified resource identifier (account:kind:identifier).
  name: id
  type: string
- description: Resource identifier of the owner role.
  name: owner
  type: string
- description: ''
  name: permissions
  type: array
- description: ''
  name: annotations
  type: array
- description: ''
  name: policy_versions
  type: array
provider_name: CyberArk
provider_slug: cyberark
schema_file: json-schema/cyberark-conjur-resource-schema.json
slug: cyberark-conjur-resource
source_filename: cyberark-conjur-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cyberark/refs/heads/main/json-schema/cyberark-conjur-resource-schema.json\",\n  \"title\": \"ConjurResource\",\n  \"description\": \"A managed object in Conjur policy (user, host, group, layer, variable, policy, or webservice).\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified resource identifier (account:kind:identifier).\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Resource identifier of the owner role.\"\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"privilege\": { \"type\": \"string\" },\n          \"role\": { \"type\": \"string\" },\n          \"policy\": { \"type\": \"string\" }\n        }\n\
  \      }\n    },\n    \"annotations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": { \"type\": \"string\" },\n          \"value\": { \"type\": \"string\" },\n          \"policy\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"policy_versions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"version\": { \"type\": \"integer\" },\n          \"created_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n          \"policy_text\": { \"type\": \"string\" },\n          \"policy_sha256\": { \"type\": \"string\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cyberark/refs/heads/main/json-schema/cyberark-conjur-resource-schema.json
tags:
- Authentication
- Cloud Security
- Conjur
- Credential Vault
- DevOps Secrets
- Endpoint Privilege Management
- Identity Security
- Machine Identity
- MFA
- OpenAPI
- PAM
- Privileged Access
- Privileged Access Management
- Secrets Management
- Session Management
- SSO
- Vault
- Zero Trust
title: ConjurResource
---
