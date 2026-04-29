---
description: A single comment attached to a problem.
layout: schema
name: Comment
properties_list:
- description: The unique identifier of the comment.
  name: id
  type: string
- description: The Unix timestamp in milliseconds when the comment was created.
  name: createdAtTimestamp
  type: integer
- description: The display name of the user who created the comment.
  name: authorName
  type: string
- description: The text content of the comment.
  name: content
  type: string
- description: Optional context reference attached to the comment.
  name: context
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-problems-v2-comment-schema.json
slug: dynatrace-problems-v2-comment
source_filename: dynatrace-problems-v2-comment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A single comment attached to a problem.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the comment.\",\n      \"example\": \"abc123\"\n    },\n    \"createdAtTimestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"The Unix timestamp in milliseconds when the comment was created.\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993\n    },\n    \"authorName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the user who created the comment.\",\n      \"example\": \"Production Service\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The text content of the comment.\",\n      \"example\": \"example-value\"\n    },\n    \"context\": {\n      \"type\": \"string\",\n      \"description\": \"Optional context reference attached to the comment.\",\n      \"example\": \"example-value\"\
  \n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Comment\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-problems-v2-comment-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: Comment
---
