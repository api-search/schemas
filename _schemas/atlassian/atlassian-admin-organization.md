---
description: Represents an Atlassian organization.
layout: schema
name: Organization
properties_list:
- description: The unique identifier of the organization.
  name: id
  type: string
- description: The resource type.
  name: type
  type: string
- description: The attributes of the organization.
  name: attributes
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-organization-schema.json
slug: atlassian-admin-organization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Organization\",\n  \"type\": \"object\",\n  \"description\": \"Represents an Atlassian organization.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the organization.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"The attributes of the organization.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-organization-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: Organization
---
