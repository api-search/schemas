---
description: An operation to perform on a field value.
layout: schema
name: FieldUpdateOperation
properties_list:
- description: Value to add to the field.
  name: add
  type: string
- description: Value to remove from the field.
  name: remove
  type: string
- description: Value to set the field to.
  name: set
  type: string
- description: Value to edit in the field.
  name: edit
  type: string
- description: Value to copy to the field.
  name: copy
  type: string
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-field-update-operation-schema.json
slug: jira-cloud-platform-rest-field-update-operation
source_filename: jira-cloud-platform-rest-field-update-operation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FieldUpdateOperation\",\n  \"type\": \"object\",\n  \"description\": \"An operation to perform on a field value.\",\n  \"properties\": {\n    \"add\": {\n      \"type\": \"string\",\n      \"description\": \"Value to add to the field.\"\n    },\n    \"remove\": {\n      \"type\": \"string\",\n      \"description\": \"Value to remove from the field.\"\n    },\n    \"set\": {\n      \"type\": \"string\",\n      \"description\": \"Value to set the field to.\"\n    },\n    \"edit\": {\n      \"type\": \"string\",\n      \"description\": \"Value to edit in the field.\"\n    },\n    \"copy\": {\n      \"type\": \"string\",\n      \"description\": \"Value to copy to the field.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-field-update-operation-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: FieldUpdateOperation
---
