---
description: Core and extended document properties for an Open XML Word document.
layout: schema
name: OpenXmlDocumentProperties
properties_list:
- description: Document title.
  name: title
  type: string
- description: Document subject.
  name: subject
  type: string
- description: Document creator/author.
  name: creator
  type: string
- description: Document description.
  name: description
  type: string
- description: Document keywords.
  name: keywords
  type: string
- description: Document category.
  name: category
  type: string
- description: Creation timestamp.
  name: created
  type: string
- description: Last modified timestamp.
  name: modified
  type: string
- description: Revision number.
  name: revision
  type: string
- description: Application that created the document.
  name: application
  type: string
- description: Total editing time in minutes.
  name: totalTime
  type: integer
- description: Number of pages.
  name: pages
  type: integer
- description: Number of words.
  name: words
  type: integer
- description: Number of characters.
  name: characters
  type: integer
provider_name: Microsoft Word
provider_slug: microsoft-word
schema_file: json-schema/open-xml-sdk-document-properties-schema.json
slug: open-xml-sdk-document-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/open-xml-sdk-document-properties-schema.json\",\n  \"title\": \"OpenXmlDocumentProperties\",\n  \"description\": \"Core and extended document properties for an Open XML Word document.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Document title.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Document subject.\"\n    },\n    \"creator\": {\n      \"type\": \"string\",\n      \"description\": \"Document creator/author.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Document description.\"\n    },\n    \"keywords\": {\n      \"type\": \"string\",\n      \"description\": \"Document keywords.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"Document category.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp.\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modified timestamp.\"\n    },\n    \"revision\": {\n      \"type\": \"string\",\n      \"description\": \"Revision number.\"\n    },\n    \"application\": {\n      \"type\": \"string\",\n      \"description\": \"Application that created the document.\"\n    },\n    \"totalTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Total editing time in minutes.\"\n    },\n    \"pages\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of pages.\"\n    },\n    \"words\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of words.\"\n    },\n    \"characters\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of characters.\"\n    }\n\
  \  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/open-xml-sdk-document-properties-schema.json
tags:
- Documents
- Microsoft 365
- Office
- Productivity
- Word Processing
title: OpenXmlDocumentProperties
---
