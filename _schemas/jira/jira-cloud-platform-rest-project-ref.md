---
description: A reference to a Jira project.
layout: schema
name: ProjectRef
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: key
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: projectTypeKey
  type: string
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-project-ref-schema.json
slug: jira-cloud-platform-rest-project-ref
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProjectRef\",\n  \"type\": \"object\",\n  \"description\": \"A reference to a Jira project.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"projectTypeKey\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-project-ref-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: ProjectRef
---
