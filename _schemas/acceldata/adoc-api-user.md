---
description: A user in the Acceldata platform
layout: schema
name: User
properties_list:
- description: User identifier
  name: id
  type: string
- description: User email address
  name: email
  type: string
- description: User full name
  name: name
  type: string
- description: Assigned role
  name: role
  type: string
- description: User account status
  name: status
  type: string
- description: Account creation timestamp
  name: createdAt
  type: string
provider_name: Acceldata
provider_slug: acceldata
schema_file: json-schema/adoc-api-user-schema.json
slug: adoc-api-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/user.json\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"description\": \"A user in the Acceldata platform\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"User identifier\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"User email address\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"User full name\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Assigned role\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"User account status\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"invited\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Account\
  \ creation timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-user-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: User
---
