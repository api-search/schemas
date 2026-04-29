---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: Numeric error code
  name: errorCode
  type: integer
- description: Human-readable error description
  name: errorMessage
  type: string
- description: Additional error details
  name: details
  type: array
provider_name: Veritas NetBackup
provider_slug: veritas-netbackup
schema_file: json-schema/veritas-netbackup-rest-error-response-schema.json
slug: veritas-netbackup-rest-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric error code\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error description\"\n    },\n    \"details\": {\n      \"type\": \"array\",\n      \"description\": \"Additional error details\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-netbackup/refs/heads/main/json-schema/veritas-netbackup-rest-error-response-schema.json
tags:
- Backup
- Data Protection
- Disaster Recovery
- Enterprise
- Recovery
- Storage
title: ErrorResponse
---
