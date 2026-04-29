---
description: Request body for performing an issue transition.
layout: schema
name: IssueTransitionRequest
properties_list:
- description: A map of field ID to field value to set during the transition.
  name: fields
  type: object
- description: A map of operations to perform on issue fields during the transition.
  name: update
  type: object
- description: Metadata about the history entry.
  name: historyMetadata
  type: object
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-issue-transition-request-schema.json
slug: jira-cloud-platform-rest-issue-transition-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IssueTransitionRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for performing an issue transition.\",\n  \"properties\": {\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"A map of field ID to field value to set during the transition.\"\n    },\n    \"update\": {\n      \"type\": \"object\",\n      \"description\": \"A map of operations to perform on issue fields during the transition.\"\n    },\n    \"historyMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about the history entry.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-issue-transition-request-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: IssueTransitionRequest
---
