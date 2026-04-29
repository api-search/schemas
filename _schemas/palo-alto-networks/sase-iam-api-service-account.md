---
description: ServiceAccount schema from Palo Alto Networks SASE IAM Service API
layout: schema
name: ServiceAccount
properties_list:
- description: Unique identifier of the service account.
  name: id
  type: string
- description: Unique name of the service account within the TSG.
  name: name
  type: string
- description: Human-readable display name.
  name: display_name
  type: string
- description: Description of the service account's purpose.
  name: description
  type: string
- description: Tenant Service Group ID this service account belongs to.
  name: tsg_id
  type: string
- description: Number of active credential keys for this service account.
  name: key_count
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-iam-api-service-account-schema.json
slug: sase-iam-api-service-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceAccount\",\n  \"description\": \"ServiceAccount schema from Palo Alto Networks SASE IAM Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-iam-api-service-account-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the service account.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the service account within the TSG.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the service account's purpose.\"\n    },\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant Service\
  \ Group ID this service account belongs to.\"\n    },\n    \"key_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active credential keys for this service account.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-iam-api-service-account-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ServiceAccount
---
