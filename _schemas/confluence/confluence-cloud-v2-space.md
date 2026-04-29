---
description: Represents a Confluence space.
layout: schema
name: Space
properties_list:
- description: The unique identifier of the space.
  name: id
  type: string
- description: The key of the space, used in URLs.
  name: key
  type: string
- description: The name of the space.
  name: name
  type: string
- description: The type of space.
  name: type
  type: string
- description: The status of the space.
  name: status
  type: string
- description: The Atlassian account ID of the space creator.
  name: authorId
  type: string
- description: The ISO 8601 timestamp when the space was created.
  name: createdAt
  type: string
- description: The ID of the space homepage.
  name: homepageId
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-space-schema.json
slug: confluence-cloud-v2-space
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Space\",\n  \"type\": \"object\",\n  \"description\": \"Represents a Confluence space.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the space.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the space, used in URLs.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the space.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of space.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the space.\"\n    },\n    \"authorId\": {\n      \"type\": \"string\",\n      \"description\": \"The Atlassian account ID of the space creator.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 8601 timestamp when the space\
  \ was created.\"\n    },\n    \"homepageId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the space homepage.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-space-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: Space
---
