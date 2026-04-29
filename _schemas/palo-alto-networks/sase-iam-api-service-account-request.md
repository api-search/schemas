---
description: ServiceAccountRequest schema from Palo Alto Networks SASE IAM Service API
layout: schema
name: ServiceAccountRequest
properties_list:
- description: Unique name for the service account within the TSG.
  name: name
  type: string
- description: Human-readable display name.
  name: display_name
  type: string
- description: Description of the service account's purpose.
  name: description
  type: string
- description: Tenant Service Group ID to create this service account in.
  name: tsg_id
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-iam-api-service-account-request-schema.json
slug: sase-iam-api-service-account-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceAccountRequest\",\n  \"description\": \"ServiceAccountRequest schema from Palo Alto Networks SASE IAM Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-iam-api-service-account-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name for the service account within the TSG.\",\n      \"pattern\": \"^[a-z][a-z0-9-]{0,63}$\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the service account's purpose.\"\n    },\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant Service Group ID to create this service account in.\"\n\
  \    }\n  },\n  \"required\": [\n    \"name\",\n    \"tsg_id\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-iam-api-service-account-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ServiceAccountRequest
---
