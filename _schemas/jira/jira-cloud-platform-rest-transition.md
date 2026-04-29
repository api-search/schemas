---
description: A workflow transition.
layout: schema
name: Transition
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: hasScreen
  type: boolean
- description: ''
  name: isGlobal
  type: boolean
- description: ''
  name: isInitial
  type: boolean
- description: ''
  name: isConditional
  type: boolean
- description: Fields available during the transition.
  name: fields
  type: object
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-transition-schema.json
slug: jira-cloud-platform-rest-transition
source_filename: jira-cloud-platform-rest-transition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Transition\",\n  \"type\": \"object\",\n  \"description\": \"A workflow transition.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"hasScreen\": {\n      \"type\": \"boolean\"\n    },\n    \"isGlobal\": {\n      \"type\": \"boolean\"\n    },\n    \"isInitial\": {\n      \"type\": \"boolean\"\n    },\n    \"isConditional\": {\n      \"type\": \"boolean\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Fields available during the transition.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-transition-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Transition
---
