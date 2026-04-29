---
description: A user name object containing given, family, and full name.
layout: schema
name: UserName
properties_list:
- description: The user first name. Required when creating a user account.
  name: givenName
  type: string
- description: The user last name. Required when creating a user account.
  name: familyName
  type: string
- description: The user full name formed by concatenating first and last name values.
  name: fullName
  type: string
- description: The user display name.
  name: displayName
  type: string
provider_name: Google Workspace
provider_slug: google-workspace
schema_file: json-schema/admin-sdk-directory-user-name-schema.json
slug: admin-sdk-directory-user-name
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserName\",\n  \"type\": \"object\",\n  \"description\": \"A user name object containing given, family, and full name.\",\n  \"properties\": {\n    \"givenName\": {\n      \"type\": \"string\",\n      \"description\": \"The user first name. Required when creating a user account.\"\n    },\n    \"familyName\": {\n      \"type\": \"string\",\n      \"description\": \"The user last name. Required when creating a user account.\"\n    },\n    \"fullName\": {\n      \"type\": \"string\",\n      \"description\": \"The user full name formed by concatenating first and last name values.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The user display name.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-workspace/refs/heads/main/json-schema/admin-sdk-directory-user-name-schema.json
tags:
- Calendar
- Collaboration
- Email
- Productivity
- Storage
- Video Conferencing
title: UserName
---
