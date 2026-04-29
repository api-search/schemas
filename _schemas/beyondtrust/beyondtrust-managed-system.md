---
description: A system registered in BeyondTrust Password Safe.
layout: schema
name: ManagedSystem
properties_list:
- description: Unique identifier of the managed system.
  name: ManagedSystemID
  type: integer
- description: Name of the system.
  name: SystemName
  type: string
- description: IP address of the system.
  name: IPAddress
  type: string
- description: Operating system platform.
  name: Platform
  type: string
- description: Network hostname or FQDN.
  name: NetworkAddress
  type: string
- description: Contact email for this system.
  name: ContactEmail
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-managed-system-schema.json
slug: beyondtrust-managed-system
source_filename: beyondtrust-managed-system-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-managed-system-schema.json\",\n  \"title\": \"ManagedSystem\",\n  \"description\": \"A system registered in BeyondTrust Password Safe.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ManagedSystemID\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier of the managed system.\",\n      \"example\": 10\n    },\n    \"SystemName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the system.\",\n      \"example\": \"prod-server-01\"\n    },\n    \"IPAddress\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the system.\",\n      \"example\": \"10.1.1.10\"\n    },\n    \"Platform\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system platform.\",\n      \"enum\": [\n        \"Windows\",\n        \"Linux\"\
  ,\n        \"Unix\",\n        \"macOS\"\n      ],\n      \"example\": \"Windows\"\n    },\n    \"NetworkAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Network hostname or FQDN.\",\n      \"example\": \"prod-server-01.example.com\"\n    },\n    \"ContactEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"nullable\": true,\n      \"description\": \"Contact email for this system.\",\n      \"example\": \"admin@example.com\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-managed-system-schema.json
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: ManagedSystem
---
