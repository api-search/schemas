---
description: A reference to an issue.
layout: schema
name: IssueRef
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: key
  type: string
- description: ''
  name: self
  type: string
- description: ''
  name: fields
  type: object
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-issue-ref-schema.json
slug: jira-cloud-platform-rest-issue-ref
source_filename: jira-cloud-platform-rest-issue-ref-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IssueRef\",\n  \"type\": \"object\",\n  \"description\": \"A reference to an issue.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"fields\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-issue-ref-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: IssueRef
---
