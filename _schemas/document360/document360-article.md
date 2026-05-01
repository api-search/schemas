---
description: An article published in a Document360 knowledge base project version.
layout: schema
name: Document360 Article
properties_list:
- description: Unique identifier for the article.
  name: id
  type: string
- description: Title of the article.
  name: title
  type: string
- description: URL slug for the article.
  name: slug
  type: string
- description: Rendered HTML content of the article.
  name: content
  type: string
- description: Markdown source of the article.
  name: contentMarkdown
  type: string
- description: Identifier of the category this article belongs to.
  name: categoryId
  type: string
- description: Identifier of the project version containing the article.
  name: projectVersionId
  type: string
- description: Language code (e.g., en, de) for the article.
  name: languageCode
  type: string
- description: Publication status of the article (e.g., draft, published).
  name: status
  type: string
- description: Timestamp when the article was created.
  name: createdAt
  type: string
- description: Timestamp when the article was last modified.
  name: modifiedAt
  type: string
provider_name: Document360
provider_slug: document360
schema_file: json-schema/document360-article-schema.json
slug: document360-article
source_filename: document360-article-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/document360/refs/heads/main/json-schema/document360-article-schema.json\",\n  \"title\": \"Document360 Article\",\n  \"description\": \"An article published in a Document360 knowledge base project version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the article.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the article.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL slug for the article.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Rendered HTML content of the article.\"\n    },\n    \"contentMarkdown\": {\n      \"type\": \"string\",\n      \"description\": \"Markdown source of the article.\"\n    },\n    \"categoryId\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"Identifier of the category this article belongs to.\"\n    },\n    \"projectVersionId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the project version containing the article.\"\n    },\n    \"languageCode\": {\n      \"type\": \"string\",\n      \"description\": \"Language code (e.g., en, de) for the article.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Publication status of the article (e.g., draft, published).\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the article was created.\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the article was last modified.\"\n    }\n  },\n  \"required\": [\"id\", \"title\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/document360/refs/heads/main/json-schema/document360-article-schema.json
tags:
- Documentation
- Knowledge Base
- SaaS
title: Document360 Article
---
