---
description: user-name-response from GitHub API
layout: schema
name: user-name-response
properties_list:
- description: The full name, including all middle names, titles, and suffixes as appropriate, formatted for display.
  name: formatted
  type: string
- description: The family name of the user.
  name: familyName
  type: string
- description: The given name of the user.
  name: givenName
  type: string
- description: The middle name(s) of the user.
  name: middleName
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-scim-user-name-response-schema.json
slug: github-scim-user-name-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-scim-user-name-response-schema.json\",\n  \"title\": \"user-name-response\",\n  \"description\": \"user-name-response from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"formatted\": {\n      \"type\": \"string\",\n      \"description\": \"The full name, including all middle names, titles, and suffixes as appropriate, formatted for display.\",\n      \"example\": \"Ms. Mona Lisa Octocat\"\n    },\n    \"familyName\": {\n      \"type\": \"string\",\n      \"description\": \"The family name of the user.\",\n      \"example\": \"Octocat\"\n    },\n    \"givenName\": {\n      \"type\": \"string\",\n      \"description\": \"The given name of the user.\",\n      \"example\": \"Mona\"\n    },\n    \"middleName\": {\n      \"type\": \"string\",\n      \"description\": \"The middle name(s) of\
  \ the user.\",\n      \"example\": \"Lisa\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-scim-user-name-response-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: user-name-response
---
