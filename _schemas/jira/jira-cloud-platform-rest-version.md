---
description: A project version.
layout: schema
name: Version
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: archived
  type: boolean
- description: ''
  name: released
  type: boolean
- description: ''
  name: releaseDate
  type: string
- description: ''
  name: startDate
  type: string
- description: ''
  name: overdue
  type: boolean
- description: ''
  name: projectId
  type: integer
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-version-schema.json
slug: jira-cloud-platform-rest-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Version\",\n  \"type\": \"object\",\n  \"description\": \"A project version.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\"\n    },\n    \"released\": {\n      \"type\": \"boolean\"\n    },\n    \"releaseDate\": {\n      \"type\": \"string\"\n    },\n    \"startDate\": {\n      \"type\": \"string\"\n    },\n    \"overdue\": {\n      \"type\": \"boolean\"\n    },\n    \"projectId\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-version-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Version
---
