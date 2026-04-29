---
description: Invite schema from Ampersand API
layout: schema
name: Invite
properties_list:
- description: The invite ID.
  name: id
  type: string
- description: The email address of the person invited.
  name: invitedEmail
  type: string
- description: The type of entity that the person is invited to.
  name: parentType
  type: string
- description: The ID of the parent (e.g. org ID).
  name: parentId
  type: string
- description: The status of the invite.
  name: status
  type: string
- description: The time the invite was created.
  name: createTime
  type: string
- description: The time the invite was updated.
  name: updateTime
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-invite-schema.json
slug: ampersand-api-invite
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-invite-schema.json\",\n  \"title\": \"Invite\",\n  \"description\": \"Invite schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The invite ID.\"\n    },\n    \"invitedEmail\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the person invited.\"\n    },\n    \"parentType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"org\"\n      ],\n      \"description\": \"The type of entity that the person is invited to.\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the parent (e.g. org ID).\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the invite.\",\n      \"enum\": [\n\
  \        \"pending\",\n        \"accepted\",\n        \"revoked\",\n        \"expired\"\n      ]\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the invite was created.\",\n      \"format\": \"date-time\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the invite was updated.\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"invitedEmail\",\n    \"createTime\",\n    \"parentId\",\n    \"parentType\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-invite-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: Invite
---
