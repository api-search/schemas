---
description: The type of link between issues.
layout: schema
name: IssueLinkType
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: The inward description (e.g., is blocked by).
  name: inward
  type: string
- description: The outward description (e.g., blocks).
  name: outward
  type: string
- description: ''
  name: self
  type: string
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-issue-link-type-schema.json
slug: jira-cloud-platform-rest-issue-link-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IssueLinkType\",\n  \"type\": \"object\",\n  \"description\": \"The type of link between issues.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"inward\": {\n      \"type\": \"string\",\n      \"description\": \"The inward description (e.g., is blocked by).\"\n    },\n    \"outward\": {\n      \"type\": \"string\",\n      \"description\": \"The outward description (e.g., blocks).\"\n    },\n    \"self\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-issue-link-type-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: IssueLinkType
---
