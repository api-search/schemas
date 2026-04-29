---
description: JiraIntegration schema from Palo Alto Networks SaaS Security Posture Management API
layout: schema
name: JiraIntegration
properties_list:
- description: Unique identifier of the Jira integration.
  name: id
  type: string
- description: Display name for the integration.
  name: name
  type: string
- description: Base URL of the Jira server or cloud instance.
  name: jira_url
  type: string
- description: Jira project key where tickets are created.
  name: project_key
  type: string
- description: Jira issue type for created tickets (e.g., Bug, Task).
  name: issue_type
  type: string
- description: Whether the integration is actively creating tickets.
  name: enabled
  type: boolean
- description: ''
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sspm-api-jira-integration-schema.json
slug: sspm-api-jira-integration
source_filename: sspm-api-jira-integration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JiraIntegration\",\n  \"description\": \"JiraIntegration schema from Palo Alto Networks SaaS Security Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sspm-api-jira-integration-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the Jira integration.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the integration.\"\n    },\n    \"jira_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Base URL of the Jira server or cloud instance.\"\n    },\n    \"project_key\": {\n      \"type\": \"string\",\n      \"description\": \"Jira project key where tickets are created.\"\n    },\n    \"issue_type\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Jira issue type for created tickets (e.g., Bug, Task).\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the integration is actively creating tickets.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sspm-api-jira-integration-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: JiraIntegration
---
