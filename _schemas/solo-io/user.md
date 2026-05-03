---
description: A user of the Gloo developer portal, representing an authenticated identity with associated groups and permissions.
layout: schema
name: Solo.io Gloo Portal User
properties_list:
- description: Unique identifier for the user.
  name: id
  type: string
- description: Email address of the user.
  name: email
  type: string
- description: Username of the user.
  name: username
  type: string
- description: Display name of the user.
  name: name
  type: string
- description: Groups the user belongs to for access control.
  name: groups
  type: array
provider_name: Solo.io
provider_slug: solo-io
schema_file: json-schema/user.json
slug: user
source_filename: user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/solo-io/blob/main/json-schema/user.json\",\n  \"title\": \"Solo.io Gloo Portal User\",\n  \"description\": \"A user of the Gloo developer portal, representing an authenticated identity with associated groups and permissions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the user.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the user.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the user.\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\"\
  : \"Groups the user belongs to for access control.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/json-schema/user.json
tags:
- AI Gateway
- Analytics
- Automation
- Gateways
- Management
- Monetization
- Observability
- Platform
- Resiliency
- Security
- Service Mesh
- Traffic Control
title: Solo.io Gloo Portal User
---
