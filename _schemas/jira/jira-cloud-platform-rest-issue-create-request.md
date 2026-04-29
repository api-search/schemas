---
description: Request body for creating an issue.
layout: schema
name: IssueCreateRequest
properties_list:
- description: A map of operations to perform on issue fields. Each key is a field ID and the value is an array of operations.
  name: update
  type: object
- description: A map of field ID to field value for the issue. Required fields depend on the project and issue type.
  name: fields
  type: object
- description: Metadata about the history entry.
  name: historyMetadata
  type: object
- description: Entity properties to set on the issue.
  name: properties
  type: array
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-issue-create-request-schema.json
slug: jira-cloud-platform-rest-issue-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IssueCreateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating an issue.\",\n  \"properties\": {\n    \"update\": {\n      \"type\": \"object\",\n      \"description\": \"A map of operations to perform on issue fields. Each key is a field ID and the value is an array of operations.\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"A map of field ID to field value for the issue. Required fields depend on the project and issue type.\"\n    },\n    \"historyMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about the history entry.\"\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"description\": \"Entity properties to set on the issue.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-issue-create-request-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: IssueCreateRequest
---
