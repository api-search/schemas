---
description: Application schema from Palo Alto Networks SaaS Security API
layout: schema
name: Application
properties_list:
- description: Unique application identifier.
  name: id
  type: string
- description: SaaS application name (e.g., Google Drive, Microsoft SharePoint).
  name: name
  type: string
- description: Application type or category.
  name: type
  type: string
- description: Current connection status.
  name: status
  type: string
- description: Number of assets scanned for this application.
  name: asset_count
  type: integer
- description: Number of active incidents for this application.
  name: incident_count
  type: integer
- description: Timestamp when the application was connected.
  name: connected_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/saas-security-api-application-schema.json
slug: saas-security-api-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Application\",\n  \"description\": \"Application schema from Palo Alto Networks SaaS Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/saas-security-api-application-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique application identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"SaaS application name (e.g., Google Drive, Microsoft SharePoint).\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Application type or category.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"connected\",\n        \"disconnected\",\n        \"error\"\n      ],\n      \"description\": \"Current connection status.\"\n    },\n    \"asset_count\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Number of assets scanned for this application.\"\n    },\n    \"incident_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active incidents for this application.\"\n    },\n    \"connected_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the application was connected.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/saas-security-api-application-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Application
---
