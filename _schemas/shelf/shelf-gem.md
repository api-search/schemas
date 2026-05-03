---
description: A Gem is a curated, verified piece of knowledge in the Shelf platform representing a discrete answer, article, or knowledge unit.
layout: schema
name: Shelf Gem
properties_list:
- description: Unique identifier for the Gem.
  name: id
  type: string
- description: Title of the knowledge Gem.
  name: title
  type: string
- description: The full text content of the Gem.
  name: content
  type: string
- description: Lifecycle status of the Gem.
  name: status
  type: string
- description: Tags for categorizing and filtering the Gem.
  name: tags
  type: array
- description: ID of the knowledge base this Gem belongs to.
  name: knowledgeBaseId
  type: string
- description: User ID of the Gem author.
  name: authorId
  type: string
- description: ISO 8601 timestamp when the Gem was created.
  name: createdAt
  type: string
- description: ISO 8601 timestamp when the Gem was last updated.
  name: updatedAt
  type: string
- description: ISO 8601 timestamp when the Gem was published.
  name: publishedAt
  type: string
- description: ISO 639-1 language code for the Gem content.
  name: language
  type: string
- description: Number of times this Gem has been viewed.
  name: viewCount
  type: integer
- description: Number of times users marked this Gem as helpful.
  name: helpfulCount
  type: integer
- description: List of file attachments associated with the Gem.
  name: attachments
  type: array
provider_name: Shelf.io
provider_slug: shelf
schema_file: json-schema/shelf-gem-schema.json
slug: shelf-gem
source_filename: shelf-gem-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/shelf/json-schema/shelf-gem-schema.json\",\n  \"title\": \"Shelf Gem\",\n  \"description\": \"A Gem is a curated, verified piece of knowledge in the Shelf platform representing a discrete answer, article, or knowledge unit.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"title\", \"content\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the Gem.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the knowledge Gem.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The full text content of the Gem.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"draft\", \"review\", \"published\", \"archived\"],\n      \"description\": \"Lifecycle status of the Gem.\"\n    },\n    \"tags\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags for categorizing and filtering the Gem.\"\n    },\n    \"knowledgeBaseId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the knowledge base this Gem belongs to.\"\n    },\n    \"authorId\": {\n      \"type\": \"string\",\n      \"description\": \"User ID of the Gem author.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the Gem was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the Gem was last updated.\"\n    },\n    \"publishedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the Gem was published.\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"ISO 639-1 language code for the Gem content.\",\n      \"example\": \"en\"\n    },\n    \"viewCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times this Gem has been viewed.\"\n    },\n    \"helpfulCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times users marked this Gem as helpful.\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"description\": \"List of file attachments associated with the Gem.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"mimeType\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/shelf/refs/heads/main/json-schema/shelf-gem-schema.json
tags:
- Artificial Intelligence
- Contact Center
- Knowledge Management
- SaaS
- Search
title: Shelf Gem
---
