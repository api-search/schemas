---
description: The visibility restrictions for a comment.
layout: schema
name: Visibility
properties_list:
- description: ''
  name: type
  type: string
- description: The name of the group or role to restrict visibility to.
  name: value
  type: string
- description: The ID of the group or role.
  name: identifier
  type: string
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-visibility-schema.json
slug: jira-cloud-platform-rest-visibility
source_filename: jira-cloud-platform-rest-visibility-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Visibility\",\n  \"type\": \"object\",\n  \"description\": \"The visibility restrictions for a comment.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the group or role to restrict visibility to.\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the group or role.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-visibility-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Visibility
---
