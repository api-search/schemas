---
description: The result of a JQL search.
layout: schema
name: SearchResults
properties_list:
- description: The expand options applied.
  name: expand
  type: string
- description: The index of the first result returned.
  name: startAt
  type: integer
- description: The maximum number of results returned per page.
  name: maxResults
  type: integer
- description: The total number of results matching the JQL query.
  name: total
  type: integer
- description: The list of issues matching the JQL query.
  name: issues
  type: array
- description: Warning messages about the JQL query.
  name: warningMessages
  type: array
- description: Field name mapping.
  name: names
  type: object
- description: JSON Schema for each field.
  name: schema
  type: object
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-search-results-schema.json
slug: jira-cloud-platform-rest-search-results
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchResults\",\n  \"type\": \"object\",\n  \"description\": \"The result of a JQL search.\",\n  \"properties\": {\n    \"expand\": {\n      \"type\": \"string\",\n      \"description\": \"The expand options applied.\"\n    },\n    \"startAt\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the first result returned.\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of results returned per page.\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of results matching the JQL query.\"\n    },\n    \"issues\": {\n      \"type\": \"array\",\n      \"description\": \"The list of issues matching the JQL query.\"\n    },\n    \"warningMessages\": {\n      \"type\": \"array\",\n      \"description\": \"Warning messages about the JQL query.\"\n    },\n    \"names\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"Field name mapping.\"\n    },\n    \"schema\": {\n      \"type\": \"object\",\n      \"description\": \"JSON Schema for each field.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-search-results-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: SearchResults
---
