---
description: Request body for JQL search via POST.
layout: schema
name: SearchRequest
properties_list:
- description: The JQL query string.
  name: jql
  type: string
- description: The index of the first item to return (page offset).
  name: startAt
  type: integer
- description: The maximum number of items to return per page.
  name: maxResults
  type: integer
- description: 'Whether to validate the JQL query. Accepted values: strict, warn, none.'
  name: validateQuery
  type: string
- description: Fields to return for each issue.
  name: fields
  type: array
- description: Expand options for additional information.
  name: expand
  type: string
- description: Issue properties to return.
  name: properties
  type: array
- description: Whether to reference fields by keys rather than IDs.
  name: fieldsByKeys
  type: boolean
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-search-request-schema.json
slug: jira-cloud-platform-rest-search-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for JQL search via POST.\",\n  \"properties\": {\n    \"jql\": {\n      \"type\": \"string\",\n      \"description\": \"The JQL query string.\"\n    },\n    \"startAt\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the first item to return (page offset).\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of items to return per page.\"\n    },\n    \"validateQuery\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to validate the JQL query. Accepted values: strict, warn, none.\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"Fields to return for each issue.\"\n    },\n    \"expand\": {\n      \"type\": \"string\",\n      \"description\": \"Expand options for additional information.\"\n\
  \    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"Issue properties to return.\"\n    },\n    \"fieldsByKeys\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to reference fields by keys rather than IDs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-search-request-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: SearchRequest
---
