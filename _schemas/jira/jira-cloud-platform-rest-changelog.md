---
description: A paginated list of changelogs.
layout: schema
name: Changelog
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
  name: histories
  type: array
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-changelog-schema.json
slug: jira-cloud-platform-rest-changelog
source_filename: jira-cloud-platform-rest-changelog-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Changelog\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of changelogs.\",\n  \"properties\": {\n    \"startAt\": {\n      \"type\": \"integer\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\"\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"histories\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-changelog-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Changelog
---
