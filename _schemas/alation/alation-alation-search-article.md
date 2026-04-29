---
description: A catalog article or wiki page
layout: schema
name: Article
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: title
  type: string
- description: ''
  name: body
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: author
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Alation
provider_slug: alation
schema_file: json-schema/alation-alation-search-article-schema.json
slug: alation-alation-search-article
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-search-article-schema.json\",\n  \"title\": \"Article\",\n  \"description\": \"A catalog article or wiki page\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"body\": {\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"author\": {\n      \"type\": \"integer\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-search-article-schema.json
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
title: Article
---
