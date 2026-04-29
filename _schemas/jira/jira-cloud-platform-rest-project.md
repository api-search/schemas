---
description: A Jira project.
layout: schema
name: Project
properties_list:
- description: The URL of the project in the REST API.
  name: self
  type: string
- description: The ID of the project.
  name: id
  type: string
- description: The key of the project (e.g., PROJ).
  name: key
  type: string
- description: The name of the project.
  name: name
  type: string
- description: A description of the project.
  name: description
  type: string
- description: Components in the project.
  name: components
  type: array
- description: Issue types available in the project.
  name: issueTypes
  type: array
- description: A URL to the project.
  name: url
  type: string
- description: The default assignee type for the project.
  name: assigneeType
  type: string
- description: The versions defined in the project.
  name: versions
  type: array
- description: Project role URLs.
  name: roles
  type: object
- description: The project type.
  name: projectTypeKey
  type: string
- description: Whether the project is simplified (next-gen/team-managed).
  name: simplified
  type: boolean
- description: The style of the project. Classic or next-gen.
  name: style
  type: string
- description: Whether the project is archived.
  name: archived
  type: boolean
- description: Whether the project is marked as deleted.
  name: deleted
  type: boolean
- description: Insight information about the project.
  name: insight
  type: object
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-project-schema.json
slug: jira-cloud-platform-rest-project
source_filename: jira-cloud-platform-rest-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Project\",\n  \"type\": \"object\",\n  \"description\": \"A Jira project.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the project in the REST API.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the project.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the project (e.g., PROJ).\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the project.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the project.\"\n    },\n    \"components\": {\n      \"type\": \"array\",\n      \"description\": \"Components in the project.\"\n    },\n    \"issueTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Issue types available in the project.\"\n    },\n\
  \    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"A URL to the project.\"\n    },\n    \"assigneeType\": {\n      \"type\": \"string\",\n      \"description\": \"The default assignee type for the project.\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\": \"The versions defined in the project.\"\n    },\n    \"roles\": {\n      \"type\": \"object\",\n      \"description\": \"Project role URLs.\"\n    },\n    \"projectTypeKey\": {\n      \"type\": \"string\",\n      \"description\": \"The project type.\"\n    },\n    \"simplified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the project is simplified (next-gen/team-managed).\"\n    },\n    \"style\": {\n      \"type\": \"string\",\n      \"description\": \"The style of the project. Classic or next-gen.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the project is archived.\"\n    },\n    \"deleted\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Whether the project is marked as deleted.\"\n    },\n    \"insight\": {\n      \"type\": \"object\",\n      \"description\": \"Insight information about the project.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-project-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Project
---
