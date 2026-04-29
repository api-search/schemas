---
description: ''
layout: schema
name: LoginResponse
properties_list:
- description: JSON Web Token for authenticating subsequent API requests
  name: token
  type: string
- description: The token type
  name: tokenType
  type: string
- description: Token validity period in seconds
  name: validity
  type: integer
provider_name: Veritas NetBackup
provider_slug: veritas-netbackup
schema_file: json-schema/veritas-netbackup-rest-login-response-schema.json
slug: veritas-netbackup-rest-login-response
source_filename: veritas-netbackup-rest-login-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LoginResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"JSON Web Token for authenticating subsequent API requests\"\n    },\n    \"tokenType\": {\n      \"type\": \"string\",\n      \"description\": \"The token type\"\n    },\n    \"validity\": {\n      \"type\": \"integer\",\n      \"description\": \"Token validity period in seconds\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-netbackup/refs/heads/main/json-schema/veritas-netbackup-rest-login-response-schema.json
tags:
- Backup
- Data Protection
- Disaster Recovery
- Enterprise
- Recovery
- Storage
title: LoginResponse
---
