---
description: Represents a Confluence page.
layout: schema
name: Page
properties_list:
- description: The unique identifier of the page.
  name: id
  type: string
- description: The current status of the page.
  name: status
  type: string
- description: The title of the page.
  name: title
  type: string
- description: The ID of the space this page belongs to.
  name: spaceId
  type: string
- description: The ID of the parent page, if the page is nested.
  name: parentId
  type: string
- description: The type of the parent (page or space).
  name: parentType
  type: string
- description: The position of this page in the page tree relative to siblings.
  name: position
  type: integer
- description: The Atlassian account ID of the page author.
  name: authorId
  type: string
- description: The Atlassian account ID of the page owner.
  name: ownerId
  type: string
- description: The Atlassian account ID of the previous owner.
  name: lastOwnerId
  type: string
- description: The ISO 8601 timestamp when the page was created.
  name: createdAt
  type: string
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-cloud-v2-page-schema.json
slug: confluence-cloud-v2-page
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Page\",\n  \"type\": \"object\",\n  \"description\": \"Represents a Confluence page.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the page.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the page.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the page.\"\n    },\n    \"spaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the space this page belongs to.\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the parent page, if the page is nested.\"\n    },\n    \"parentType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the parent (page or space).\"\n    },\n    \"position\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"The position of this page in the page tree relative to siblings.\"\n    },\n    \"authorId\": {\n      \"type\": \"string\",\n      \"description\": \"The Atlassian account ID of the page author.\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"The Atlassian account ID of the page owner.\"\n    },\n    \"lastOwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"The Atlassian account ID of the previous owner.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 8601 timestamp when the page was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-cloud-v2-page-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: Page
---
