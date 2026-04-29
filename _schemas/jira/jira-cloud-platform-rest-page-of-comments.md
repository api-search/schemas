---
description: A paginated list of comments.
layout: schema
name: PageOfComments
properties_list:
- description: ''
  name: startAt
  type: integer
- description: ''
  name: maxResults
  type: integer
- description: ''
  name: total
  type: integer
- description: ''
  name: comments
  type: array
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-page-of-comments-schema.json
slug: jira-cloud-platform-rest-page-of-comments
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PageOfComments\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of comments.\",\n  \"properties\": {\n    \"startAt\": {\n      \"type\": \"integer\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\"\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"comments\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-page-of-comments-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: PageOfComments
---
