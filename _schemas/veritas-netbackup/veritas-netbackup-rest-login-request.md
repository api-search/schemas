---
description: ''
layout: schema
name: LoginRequest
properties_list:
- description: The authentication domain name (e.g., the NetBackup primary server hostname)
  name: domainName
  type: string
- description: The type of authentication domain
  name: domainType
  type: string
- description: The user account name
  name: userName
  type: string
- description: The user account password
  name: password
  type: string
provider_name: Veritas NetBackup
provider_slug: veritas-netbackup
schema_file: json-schema/veritas-netbackup-rest-login-request-schema.json
slug: veritas-netbackup-rest-login-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LoginRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainName\": {\n      \"type\": \"string\",\n      \"description\": \"The authentication domain name (e.g., the NetBackup primary server hostname)\"\n    },\n    \"domainType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of authentication domain\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"The user account name\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"The user account password\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-netbackup/refs/heads/main/json-schema/veritas-netbackup-rest-login-request-schema.json
tags:
- Backup
- Data Protection
- Disaster Recovery
- Enterprise
- Recovery
- Storage
title: LoginRequest
---
