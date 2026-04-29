---
description: A paginated collection of problem comments.
layout: schema
name: CommentCollection
properties_list:
- description: Cursor for the next page of results.
  name: nextPageKey
  type: string
- description: The total number of comments.
  name: totalCount
  type: integer
- description: The list of comments on this page.
  name: comments
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-problems-v2-comment-collection-schema.json
slug: dynatrace-problems-v2-comment-collection
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A paginated collection of problem comments.\",\n  \"properties\": {\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of results.\",\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of comments.\",\n      \"format\": \"int64\",\n      \"example\": 500\n    },\n    \"comments\": {\n      \"type\": \"array\",\n      \"description\": \"The list of comments on this page.\",\n      \"example\": [\n        {\n          \"id\": \"abc123\",\n          \"createdAtTimestamp\": 1718153645993,\n          \"authorName\": \"Production Service\",\n          \"content\": \"example-value\",\n          \"context\": \"example-value\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single comment attached to a problem.\",\n        \"properties\": {\n\
  \          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the comment.\",\n            \"example\": \"abc123\"\n          },\n          \"createdAtTimestamp\": {\n            \"type\": \"integer\",\n            \"description\": \"The Unix timestamp in milliseconds when the comment was created.\",\n            \"format\": \"int64\",\n            \"example\": 1718153645993\n          },\n          \"authorName\": {\n            \"type\": \"string\",\n            \"description\": \"The display name of the user who created the comment.\",\n            \"example\": \"Production Service\"\n          },\n          \"content\": {\n            \"type\": \"string\",\n            \"description\": \"The text content of the comment.\",\n            \"example\": \"example-value\"\n          },\n          \"context\": {\n            \"type\": \"string\",\n            \"description\": \"Optional context reference attached to the comment.\",\n    \
  \        \"example\": \"example-value\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommentCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-problems-v2-comment-collection-schema.json
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
title: CommentCollection
---
