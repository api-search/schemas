---
description: Schema for a Salesforce Knowledge article record.
layout: schema
name: Salesforce Knowledge Article
properties_list:
- description: Salesforce record ID for the KnowledgeArticle
  name: Id
  type: string
- description: The master article ID shared across all versions
  name: KnowledgeArticleId
  type: string
- description: Title of the knowledge article
  name: Title
  type: string
- description: URL-friendly slug used in article URLs
  name: UrlName
  type: string
- description: Short summary of the article content
  name: Summary
  type: string
- description: Current publication status of the article
  name: PublishStatus
  type: string
- description: Language code for the article (e.g., en_US, fr, de)
  name: Language
  type: string
- description: Version number of the article
  name: VersionNumber
  type: integer
- description: Whether the article is visible in the Salesforce app channel
  name: IsVisibleInApp
  type: boolean
- description: Whether the article is visible in the Public Knowledge Base channel
  name: IsVisibleInPkb
  type: boolean
- description: Whether the article is visible in the Customer Portal channel
  name: IsVisibleInCsp
  type: boolean
- description: Whether the article is visible in the Partner Portal channel
  name: IsVisibleInPrm
  type: boolean
- description: Timestamp when the article was last published
  name: LastPublishedDate
  type: string
- description: Timestamp when the article was created
  name: CreatedDate
  type: string
- description: Timestamp when the article was last modified
  name: LastModifiedDate
  type: string
- description: Salesforce ID of the user who created the article
  name: CreatedById
  type: string
- description: Salesforce ID of the article owner
  name: OwnerId
  type: string
provider_name: Salesforce Knowledge Management
provider_slug: salesforce-knowledge-management
schema_file: json-schema/salesforce-knowledge-management-article-schema.json
slug: salesforce-knowledge-management-article
source_filename: salesforce-knowledge-management-article-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/salesforce-knowledge-management/blob/main/json-schema/salesforce-knowledge-management-article-schema.json\",\n  \"title\": \"Salesforce Knowledge Article\",\n  \"description\": \"Schema for a Salesforce Knowledge article record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce record ID for the KnowledgeArticle\"\n    },\n    \"KnowledgeArticleId\": {\n      \"type\": \"string\",\n      \"description\": \"The master article ID shared across all versions\"\n    },\n    \"Title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the knowledge article\"\n    },\n    \"UrlName\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly slug used in article URLs\",\n      \"pattern\": \"^[a-z0-9-]+$\"\n    },\n    \"Summary\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Short summary of the article content\"\n    },\n    \"PublishStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current publication status of the article\",\n      \"enum\": [\"Online\", \"Draft\", \"Archived\"]\n    },\n    \"Language\": {\n      \"type\": \"string\",\n      \"description\": \"Language code for the article (e.g., en_US, fr, de)\",\n      \"examples\": [\"en_US\", \"fr\", \"de\", \"es\", \"ja\"]\n    },\n    \"VersionNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number of the article\",\n      \"minimum\": 1\n    },\n    \"IsVisibleInApp\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the article is visible in the Salesforce app channel\"\n    },\n    \"IsVisibleInPkb\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the article is visible in the Public Knowledge Base channel\"\n    },\n    \"IsVisibleInCsp\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the article is visible in the Customer Portal channel\"\n    },\n    \"IsVisibleInPrm\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the article is visible in the Partner Portal channel\"\n    },\n    \"LastPublishedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the article was last published\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the article was created\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the article was last modified\"\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce ID of the user who created the article\"\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce ID of the article owner\"\n    }\n\
  \  },\n  \"required\": [\"Title\", \"PublishStatus\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-knowledge-management/refs/heads/main/json-schema/salesforce-knowledge-management-article-schema.json
tags:
- Articles
- CRM
- Customer Service
- Documentation
- Knowledge Management
- Support
title: Salesforce Knowledge Article
---
