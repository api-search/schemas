---
description: A paginated list of worklogs.
layout: schema
name: PageOfWorklogs
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
  name: worklogs
  type: array
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-page-of-worklogs-schema.json
slug: jira-cloud-platform-rest-page-of-worklogs
source_filename: jira-cloud-platform-rest-page-of-worklogs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PageOfWorklogs\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of worklogs.\",\n  \"properties\": {\n    \"startAt\": {\n      \"type\": \"integer\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\"\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"worklogs\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-page-of-worklogs-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: PageOfWorklogs
---
