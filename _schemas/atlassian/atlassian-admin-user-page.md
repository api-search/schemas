---
description: A paginated list of users.
layout: schema
name: UserPage
properties_list:
- description: The list of users.
  name: data
  type: array
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-user-page-schema.json
slug: atlassian-admin-user-page
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserPage\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of users.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The list of users.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-user-page-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: UserPage
---
