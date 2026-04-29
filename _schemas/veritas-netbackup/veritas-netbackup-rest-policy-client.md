---
description: ''
layout: schema
name: PolicyClient
properties_list:
- description: Hostname of the client
  name: clientName
  type: string
- description: Hardware type of the client
  name: hardware
  type: string
- description: Operating system of the client
  name: operatingSystem
  type: string
- description: Client priority within the policy
  name: priority
  type: integer
provider_name: Veritas NetBackup
provider_slug: veritas-netbackup
schema_file: json-schema/veritas-netbackup-rest-policy-client-schema.json
slug: veritas-netbackup-rest-policy-client
source_filename: veritas-netbackup-rest-policy-client-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PolicyClient\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientName\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the client\"\n    },\n    \"hardware\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware type of the client\"\n    },\n    \"operatingSystem\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system of the client\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Client priority within the policy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-netbackup/refs/heads/main/json-schema/veritas-netbackup-rest-policy-client-schema.json
tags:
- Backup
- Data Protection
- Disaster Recovery
- Enterprise
- Recovery
- Storage
title: PolicyClient
---
