---
description: OnboardAppRequest schema from Palo Alto Networks SaaS Security Posture Management API
layout: schema
name: OnboardAppRequest
properties_list:
- description: Application type to onboard (e.g., google_workspace, microsoft_365, salesforce).
  name: app_type
  type: string
- description: Optional display name for this application instance.
  name: display_name
  type: string
- description: Authentication credentials required to connect to the application.
  name: credentials
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sspm-api-onboard-app-request-schema.json
slug: sspm-api-onboard-app-request
source_filename: sspm-api-onboard-app-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OnboardAppRequest\",\n  \"description\": \"OnboardAppRequest schema from Palo Alto Networks SaaS Security Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sspm-api-onboard-app-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"app_type\": {\n      \"type\": \"string\",\n      \"description\": \"Application type to onboard (e.g., google_workspace, microsoft_365, salesforce).\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Optional display name for this application instance.\"\n    },\n    \"credentials\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication credentials required to connect to the application.\",\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\n    \"app_type\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sspm-api-onboard-app-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: OnboardAppRequest
---
