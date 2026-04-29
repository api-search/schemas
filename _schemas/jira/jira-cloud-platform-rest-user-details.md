---
description: A Jira user.
layout: schema
name: UserDetails
properties_list:
- description: The URL of the user in the REST API.
  name: self
  type: string
- description: The account ID of the user, which uniquely identifies the user across all Atlassian products.
  name: accountId
  type: string
- description: The email address of the user (may not be available depending on privacy settings).
  name: emailAddress
  type: string
- description: The display name of the user.
  name: displayName
  type: string
- description: Whether the user account is active.
  name: active
  type: boolean
- description: The time zone of the user.
  name: timeZone
  type: string
- description: The type of account.
  name: accountType
  type: string
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-user-details-schema.json
slug: jira-cloud-platform-rest-user-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserDetails\",\n  \"type\": \"object\",\n  \"description\": \"A Jira user.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the user in the REST API.\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account ID of the user, which uniquely identifies the user across all Atlassian products.\"\n    },\n    \"emailAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the user (may not be available depending on privacy settings).\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the user.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is active.\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\",\n      \"description\": \"The time zone of\
  \ the user.\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of account.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-user-details-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: UserDetails
---
