---
description: An Amazon Kendra FAQ list associated with a search index.
layout: schema
name: Faq
properties_list:
- description: The identifier of the FAQ.
  name: Id
  type: string
- description: The name of the FAQ.
  name: Name
  type: string
- description: The status of the FAQ.
  name: Status
  type: string
- description: The format of the FAQ file.
  name: FileFormat
  type: string
- description: When the FAQ was created.
  name: CreatedAt
  type: string
- description: When the FAQ was last updated.
  name: UpdatedAt
  type: string
provider_name: Amazon Kendra
provider_slug: amazon-kendra
schema_file: json-schema/amazon-kendra-faq-schema.json
slug: amazon-kendra-faq
source_filename: amazon-kendra-faq-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/json-schema/amazon-kendra-faq-schema.json\",\n  \"title\": \"Faq\",\n  \"description\": \"An Amazon Kendra FAQ list associated with a search index.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the FAQ.\",\n      \"example\": \"faq-abc12345\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the FAQ.\",\n      \"example\": \"product-faqs\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATING\",\n        \"UPDATING\",\n        \"ACTIVE\",\n        \"DELETING\",\n        \"FAILED\"\n      ],\n      \"description\": \"The status of the FAQ.\",\n      \"example\": \"ACTIVE\"\n    },\n    \"FileFormat\": {\n      \"type\": \"string\",\n      \"enum\"\
  : [\n        \"CSV\",\n        \"CSV_WITH_HEADER\",\n        \"JSON\"\n      ],\n      \"description\": \"The format of the FAQ file.\",\n      \"example\": \"CSV\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the FAQ was created.\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the FAQ was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/json-schema/amazon-kendra-faq-schema.json
tags:
- AI
- AWS
- Enterprise Search
- Knowledge Management
- Machine Learning
- Natural Language
title: Faq
---
