---
description: Incident schema from Palo Alto Networks SaaS Security API
layout: schema
name: Incident
properties_list:
- description: Unique incident identifier.
  name: id
  type: string
- description: Summary title of the incident.
  name: title
  type: string
- description: Detailed description of the security incident.
  name: description
  type: string
- description: Current incident status.
  name: status
  type: string
- description: Incident severity level.
  name: severity
  type: string
- description: ID of the SaaS application where the incident occurred.
  name: app_id
  type: string
- description: Name of the SaaS application.
  name: app_name
  type: string
- description: Name of the policy that triggered the incident.
  name: policy_name
  type: string
- description: IDs of assets involved in the incident.
  name: affected_assets
  type: array
- description: User IDs of users involved in the incident.
  name: affected_users
  type: array
- description: User ID of the assigned analyst.
  name: assignee_id
  type: string
- description: Timestamp when the incident was detected.
  name: created_at
  type: string
- description: Timestamp of the most recent update.
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/saas-security-api-incident-schema.json
slug: saas-security-api-incident
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Incident\",\n  \"description\": \"Incident schema from Palo Alto Networks SaaS Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/saas-security-api-incident-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique incident identifier.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Summary title of the incident.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the security incident.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"new\",\n        \"in_progress\",\n        \"resolved\",\n        \"dismissed\"\n      ],\n      \"description\": \"Current incident status.\"\n    },\n    \"severity\": {\n  \
  \    \"type\": \"string\",\n      \"enum\": [\n        \"low\",\n        \"medium\",\n        \"high\",\n        \"critical\"\n      ],\n      \"description\": \"Incident severity level.\"\n    },\n    \"app_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the SaaS application where the incident occurred.\"\n    },\n    \"app_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the SaaS application.\"\n    },\n    \"policy_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the policy that triggered the incident.\"\n    },\n    \"affected_assets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IDs of assets involved in the incident.\"\n    },\n    \"affected_users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"User IDs of users involved in the incident.\"\n    },\n    \"assignee_id\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"User ID of the assigned analyst.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the incident was detected.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent update.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/saas-security-api-incident-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Incident
---
