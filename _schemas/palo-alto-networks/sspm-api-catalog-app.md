---
description: CatalogApp schema from Palo Alto Networks SaaS Security Posture Management API
layout: schema
name: CatalogApp
properties_list:
- description: Application type identifier used for onboarding.
  name: app_type
  type: string
- description: Human-readable application name.
  name: display_name
  type: string
- description: Application category (e.g., collaboration, crm, storage).
  name: category
  type: string
- description: Number of posture checks available for this application.
  name: check_count
  type: integer
- description: Compliance frameworks covered by checks for this application.
  name: compliance_frameworks
  type: array
- description: URL to the application logo.
  name: logo_url
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sspm-api-catalog-app-schema.json
slug: sspm-api-catalog-app
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CatalogApp\",\n  \"description\": \"CatalogApp schema from Palo Alto Networks SaaS Security Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sspm-api-catalog-app-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"app_type\": {\n      \"type\": \"string\",\n      \"description\": \"Application type identifier used for onboarding.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable application name.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Application category (e.g., collaboration, crm, storage).\"\n    },\n    \"check_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of posture checks available for this application.\"\n    },\n    \"compliance_frameworks\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Compliance frameworks covered by checks for this application.\"\n    },\n    \"logo_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the application logo.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sspm-api-catalog-app-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CatalogApp
---
