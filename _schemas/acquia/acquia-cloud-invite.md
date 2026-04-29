---
description: Details an invite.
layout: schema
name: Invite
properties_list:
- description: The unique identifier of the Invite.
  name: uuid
  type: string
- description: The invitee email address.
  name: email
  type: string
- description: The invite creation time.
  name: created_at
  type: string
- description: The invite token.
  name: token
  type: string
- description: ''
  name: flags
  type: object
- description: ''
  name: author
  type: object
- description: ''
  name: organization
  type: object
- description: ''
  name: team
  type: object
- description: List of applications the invite will grant the invitee.
  name: applications
  type: array
- description: List of roles the invite will grant the invitee.
  name: roles
  type: array
- description: ''
  name: _links
  type: object
provider_name: Acquia
provider_slug: acquia
schema_file: json-schema/acquia-cloud-invite-schema.json
slug: acquia-cloud-invite
source_filename: acquia-cloud-invite-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-invite-schema.json\",\n  \"title\": \"Invite\",\n  \"description\": \"Details an invite.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the Invite.\",\n      \"format\": \"uuid\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The invitee email address.\",\n      \"format\": \"email\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"The invite creation time.\",\n      \"format\": \"date-time\"\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The invite token.\"\n    },\n    \"flags\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_invite-flags\"\n    },\n    \"author\": {\n \
  \     \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_user-stub\"\n    },\n    \"organization\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_organization-stub\"\n    },\n    \"team\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_team-stub\"\n    },\n    \"applications\": {\n      \"type\": \"array\",\n      \"description\": \"List of applications the invite will grant the invitee.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_application-stub\"\n      }\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"description\": \"List of roles the invite will grant the invitee.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_role-stub\"\n      }\n    },\n    \"_links\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_links\"\n    }\n  },\n  \"required\": [\n    \"uuid\",\n    \"email\",\n  \
  \  \"created_at\",\n    \"token\",\n    \"flags\",\n    \"author\",\n    \"_links\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-invite-schema.json
tags:
- Content
- Experience
title: Invite
---
