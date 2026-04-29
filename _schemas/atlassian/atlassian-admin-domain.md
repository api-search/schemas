---
description: Represents a verified domain associated with an organization.
layout: schema
name: Domain
properties_list:
- description: The unique identifier of the domain.
  name: id
  type: string
- description: The resource type.
  name: type
  type: string
- description: The attributes of the domain.
  name: attributes
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-domain-schema.json
slug: atlassian-admin-domain
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Domain\",\n  \"type\": \"object\",\n  \"description\": \"Represents a verified domain associated with an organization.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the domain.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"The attributes of the domain.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-domain-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: Domain
---
