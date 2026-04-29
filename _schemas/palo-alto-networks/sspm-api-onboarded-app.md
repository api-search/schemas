---
description: OnboardedApp schema from Palo Alto Networks SaaS Security Posture Management API
layout: schema
name: OnboardedApp
properties_list:
- description: Unique identifier for the onboarded application.
  name: app_id
  type: string
- description: Application type identifier (e.g., google_workspace, microsoft_365).
  name: app_type
  type: string
- description: Human-readable name for the onboarded application instance.
  name: display_name
  type: string
- description: Current connection status.
  name: status
  type: string
- description: Tenant or domain identifier within the SaaS application.
  name: tenant_id
  type: string
- description: Summary counts of posture check results by severity.
  name: check_summary
  type: object
- description: Timestamp of the most recent posture scan.
  name: last_scanned_at
  type: string
- description: Timestamp when the application was onboarded.
  name: onboarded_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sspm-api-onboarded-app-schema.json
slug: sspm-api-onboarded-app
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OnboardedApp\",\n  \"description\": \"OnboardedApp schema from Palo Alto Networks SaaS Security Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sspm-api-onboarded-app-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"app_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the onboarded application.\"\n    },\n    \"app_type\": {\n      \"type\": \"string\",\n      \"description\": \"Application type identifier (e.g., google_workspace, microsoft_365).\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the onboarded application instance.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"connected\",\n        \"disconnected\",\n        \"pending\",\n        \"\
  error\"\n      ],\n      \"description\": \"Current connection status.\"\n    },\n    \"tenant_id\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant or domain identifier within the SaaS application.\"\n    },\n    \"check_summary\": {\n      \"type\": \"object\",\n      \"description\": \"Summary counts of posture check results by severity.\",\n      \"properties\": {\n        \"critical\": {\n          \"type\": \"integer\"\n        },\n        \"high\": {\n          \"type\": \"integer\"\n        },\n        \"medium\": {\n          \"type\": \"integer\"\n        },\n        \"low\": {\n          \"type\": \"integer\"\n        },\n        \"pass\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"last_scanned_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent posture scan.\"\n    },\n    \"onboarded_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n  \
  \    \"description\": \"Timestamp when the application was onboarded.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sspm-api-onboarded-app-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: OnboardedApp
---
