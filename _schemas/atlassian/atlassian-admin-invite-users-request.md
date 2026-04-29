---
description: Request body for inviting users to the organization.
layout: schema
name: InviteUsersRequest
properties_list:
- description: Email addresses of users to invite.
  name: emails
  type: array
- description: The directory to add the invited users to.
  name: directoryId
  type: string
- description: Groups to assign the invited users to.
  name: groupIds
  type: array
- description: Application roles to assign to the invited users.
  name: roleAssignments
  type: array
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-invite-users-request-schema.json
slug: atlassian-admin-invite-users-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InviteUsersRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for inviting users to the organization.\",\n  \"properties\": {\n    \"emails\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses of users to invite.\"\n    },\n    \"directoryId\": {\n      \"type\": \"string\",\n      \"description\": \"The directory to add the invited users to.\"\n    },\n    \"groupIds\": {\n      \"type\": \"array\",\n      \"description\": \"Groups to assign the invited users to.\"\n    },\n    \"roleAssignments\": {\n      \"type\": \"array\",\n      \"description\": \"Application roles to assign to the invited users.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-invite-users-request-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: InviteUsersRequest
---
