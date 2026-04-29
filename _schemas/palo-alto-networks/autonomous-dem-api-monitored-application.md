---
description: MonitoredApplication schema from Palo Alto Networks Autonomous DEM API
layout: schema
name: MonitoredApplication
properties_list:
- description: Unique application identifier.
  name: app_id
  type: string
- description: Application name.
  name: name
  type: string
- description: Application category (e.g., Collaboration, Productivity, Security).
  name: category
  type: string
- description: Whether the application is a SaaS or internal application.
  name: type
  type: string
- description: Primary URL for the application.
  name: url
  type: string
- description: Number of synthetic tests configured for this application.
  name: test_count
  type: integer
- description: Number of users with active monitoring for this application.
  name: monitored_users
  type: integer
- description: Timestamp when the application was added to monitoring.
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/autonomous-dem-api-monitored-application-schema.json
slug: autonomous-dem-api-monitored-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MonitoredApplication\",\n  \"description\": \"MonitoredApplication schema from Palo Alto Networks Autonomous DEM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/autonomous-dem-api-monitored-application-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"app_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique application identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Application name.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Application category (e.g., Collaboration, Productivity, Security).\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"saas\",\n        \"internal\"\n      ],\n      \"description\": \"Whether the application is a SaaS or internal application.\"\n\
  \    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Primary URL for the application.\"\n    },\n    \"test_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of synthetic tests configured for this application.\"\n    },\n    \"monitored_users\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of users with active monitoring for this application.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the application was added to monitoring.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/autonomous-dem-api-monitored-application-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MonitoredApplication
---
