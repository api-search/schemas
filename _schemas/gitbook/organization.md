---
description: An organization in GitBook that groups users, spaces, and collections under a shared account with roles and permissions.
layout: schema
name: GitBook Organization
properties_list:
- description: The unique identifier of the organization.
  name: id
  type: string
- description: The display name of the organization.
  name: title
  type: string
- description: The timestamp when the organization was created.
  name: createdAt
  type: string
- description: The timestamp when the organization was last updated.
  name: updatedAt
  type: string
- description: URLs associated with the organization.
  name: urls
  type: object
provider_name: GitBook
provider_slug: gitbook
schema_file: json-schema/organization.json
slug: organization
source_filename: organization.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gitbook/blob/main/json-schema/organization.json\",\n  \"title\": \"GitBook Organization\",\n  \"description\": \"An organization in GitBook that groups users, spaces, and collections under a shared account with roles and permissions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the organization.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the organization.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the organization was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the organization was last updated.\"\n    },\n\
  \    \"urls\": {\n      \"type\": \"object\",\n      \"description\": \"URLs associated with the organization.\",\n      \"properties\": {\n        \"app\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the organization in the GitBook app.\"\n        },\n        \"published\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the organization's published site.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/json-schema/organization.json
tags:
- Content
- Documentation
- Experience
- Integrations
- Platform
- SDKs
title: GitBook Organization
---
