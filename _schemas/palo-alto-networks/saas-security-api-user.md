---
description: User schema from Palo Alto Networks SaaS Security API
layout: schema
name: User
properties_list:
- description: Unique user identifier.
  name: id
  type: string
- description: User email address.
  name: email
  type: string
- description: User display name.
  name: display_name
  type: string
- description: SaaS application ID the user belongs to.
  name: app_id
  type: string
- description: Type of user account.
  name: account_type
  type: string
- description: Timestamp of the user's most recent activity.
  name: last_activity
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/saas-security-api-user-schema.json
slug: saas-security-api-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"description\": \"User schema from Palo Alto Networks SaaS Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/saas-security-api-user-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique user identifier.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"User email address.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"User display name.\"\n    },\n    \"app_id\": {\n      \"type\": \"string\",\n      \"description\": \"SaaS application ID the user belongs to.\"\n    },\n    \"account_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"internal\",\n        \"external\",\n        \"service\"\n      ],\n\
  \      \"description\": \"Type of user account.\"\n    },\n    \"last_activity\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the user's most recent activity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/saas-security-api-user-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: User
---
