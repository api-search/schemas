---
description: JiraIntegrationRequest schema from Palo Alto Networks SaaS Security Posture Management API
layout: schema
name: JiraIntegrationRequest
properties_list:
- description: Display name for this integration.
  name: name
  type: string
- description: Base URL of the Jira server or cloud instance.
  name: jira_url
  type: string
- description: Jira project key where tickets will be created.
  name: project_key
  type: string
- description: Jira issue type (e.g., Bug, Task, Story).
  name: issue_type
  type: string
- description: Jira API token for authentication.
  name: api_token
  type: string
- description: Email address associated with the Jira API token.
  name: email
  type: string
- description: Mapping from SSPM severity levels to Jira priorities.
  name: severity_mapping
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sspm-api-jira-integration-request-schema.json
slug: sspm-api-jira-integration-request
source_filename: sspm-api-jira-integration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JiraIntegrationRequest\",\n  \"description\": \"JiraIntegrationRequest schema from Palo Alto Networks SaaS Security Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sspm-api-jira-integration-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for this integration.\"\n    },\n    \"jira_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Base URL of the Jira server or cloud instance.\"\n    },\n    \"project_key\": {\n      \"type\": \"string\",\n      \"description\": \"Jira project key where tickets will be created.\"\n    },\n    \"issue_type\": {\n      \"type\": \"string\",\n      \"description\": \"Jira issue type (e.g., Bug, Task, Story).\",\n      \"default\"\
  : \"Bug\"\n    },\n    \"api_token\": {\n      \"type\": \"string\",\n      \"description\": \"Jira API token for authentication.\",\n      \"writeOnly\": true\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address associated with the Jira API token.\"\n    },\n    \"severity_mapping\": {\n      \"type\": \"object\",\n      \"description\": \"Mapping from SSPM severity levels to Jira priorities.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"jira_url\",\n    \"project_key\",\n    \"api_token\",\n    \"email\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sspm-api-jira-integration-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: JiraIntegrationRequest
---
