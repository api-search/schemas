---
description: An individual field change within a changelog entry.
layout: schema
name: ChangeItem
properties_list:
- description: ''
  name: field
  type: string
- description: ''
  name: fieldtype
  type: string
- description: ''
  name: fieldId
  type: string
- description: ''
  name: from
  type: '[''string'', ''null'']'
- description: ''
  name: fromString
  type: '[''string'', ''null'']'
- description: ''
  name: to
  type: '[''string'', ''null'']'
- description: ''
  name: toString
  type: '[''string'', ''null'']'
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-change-item-schema.json
slug: jira-cloud-platform-rest-change-item
source_filename: jira-cloud-platform-rest-change-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChangeItem\",\n  \"type\": \"object\",\n  \"description\": \"An individual field change within a changelog entry.\",\n  \"properties\": {\n    \"field\": {\n      \"type\": \"string\"\n    },\n    \"fieldtype\": {\n      \"type\": \"string\"\n    },\n    \"fieldId\": {\n      \"type\": \"string\"\n    },\n    \"from\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"fromString\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"to\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"toString\": {\n      \"type\": \"['string', 'null']\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-change-item-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: ChangeItem
---
