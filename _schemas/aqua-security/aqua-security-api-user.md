---
description: User schema from Aqua Security API
layout: schema
name: User
properties_list:
- description: User login ID
  name: id
  type: string
- description: User display name
  name: name
  type: string
- description: User role
  name: role
  type: string
- description: User email address
  name: email
  type: string
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-user-schema.json
slug: aqua-security-api-user
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"admin\",\n      \"description\": \"User login ID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Administrator\",\n      \"description\": \"User display name\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"administrator\",\n        \"auditor\",\n        \"scanner\",\n        \"image_assurance\",\n        \"runtime_policy\"\n      ],\n      \"example\": \"administrator\",\n      \"description\": \"User role\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"example\": \"admin@example.com\",\n      \"description\": \"User email address\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-user-schema.json\"\
  ,\n  \"title\": \"User\",\n  \"description\": \"User schema from Aqua Security API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-user-schema.json
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: User
---
