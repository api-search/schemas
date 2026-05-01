---
description: A user account in GitBook with profile information including display name, email, and photo.
layout: schema
name: GitBook User
properties_list:
- description: The unique identifier of the user.
  name: id
  type: string
- description: The display name of the user.
  name: displayName
  type: string
- description: The email address of the user.
  name: email
  type: string
- description: URL to the user's profile photo.
  name: photoURL
  type: string
- description: URLs associated with the user.
  name: urls
  type: object
provider_name: GitBook
provider_slug: gitbook
schema_file: json-schema/user.json
slug: user
source_filename: user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gitbook/blob/main/json-schema/user.json\",\n  \"title\": \"GitBook User\",\n  \"description\": \"A user account in GitBook with profile information including display name, email, and photo.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the user.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the user.\"\n    },\n    \"photoURL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the user's profile photo.\"\n    },\n    \"urls\": {\n      \"type\": \"object\",\n      \"description\": \"URLs associated with the user.\",\n\
  \      \"properties\": {\n        \"app\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's profile in the GitBook app.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/json-schema/user.json
tags:
- Content
- Documentation
- Experience
- Integrations
- Platform
- SDKs
title: GitBook User
---
