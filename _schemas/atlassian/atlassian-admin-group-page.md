---
description: A paginated list of groups.
layout: schema
name: GroupPage
properties_list:
- description: The list of groups.
  name: data
  type: array
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-group-page-schema.json
slug: atlassian-admin-group-page
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupPage\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of groups.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The list of groups.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-group-page-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: GroupPage
---
