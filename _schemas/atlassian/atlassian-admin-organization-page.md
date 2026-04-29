---
description: A paginated list of organizations.
layout: schema
name: OrganizationPage
properties_list:
- description: The list of organizations.
  name: data
  type: array
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-organization-page-schema.json
slug: atlassian-admin-organization-page
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrganizationPage\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of organizations.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The list of organizations.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-organization-page-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: OrganizationPage
---
