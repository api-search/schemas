---
description: UserActivity schema from Palo Alto Networks SaaS Security API
layout: schema
name: UserActivity
properties_list:
- description: Unique activity record identifier.
  name: id
  type: string
- description: ID of the user who performed the action.
  name: user_id
  type: string
- description: SaaS application where the activity occurred.
  name: app_id
  type: string
- description: Type of action performed (e.g., file_download, share_external).
  name: action
  type: string
- description: ID of the asset involved in the activity.
  name: asset_id
  type: string
- description: Timestamp when the activity occurred.
  name: timestamp
  type: string
- description: Source IP address of the activity.
  name: ip_address
  type: string
- description: Risk level assigned to this activity.
  name: risk_level
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/saas-security-api-user-activity-schema.json
slug: saas-security-api-user-activity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserActivity\",\n  \"description\": \"UserActivity schema from Palo Alto Networks SaaS Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/saas-security-api-user-activity-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique activity record identifier.\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who performed the action.\"\n    },\n    \"app_id\": {\n      \"type\": \"string\",\n      \"description\": \"SaaS application where the activity occurred.\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Type of action performed (e.g., file_download, share_external).\"\n    },\n    \"asset_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID\
  \ of the asset involved in the activity.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the activity occurred.\"\n    },\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\": \"Source IP address of the activity.\"\n    },\n    \"risk_level\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"low\",\n        \"medium\",\n        \"high\"\n      ],\n      \"description\": \"Risk level assigned to this activity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/saas-security-api-user-activity-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: UserActivity
---
