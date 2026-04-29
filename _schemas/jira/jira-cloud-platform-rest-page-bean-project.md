---
description: A paginated list of projects.
layout: schema
name: PageBeanProject
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: nextPage
  type: string
- description: ''
  name: maxResults
  type: integer
- description: ''
  name: startAt
  type: integer
- description: ''
  name: total
  type: integer
- description: ''
  name: isLast
  type: boolean
- description: ''
  name: values
  type: array
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-page-bean-project-schema.json
slug: jira-cloud-platform-rest-page-bean-project
source_filename: jira-cloud-platform-rest-page-bean-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PageBeanProject\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of projects.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"nextPage\": {\n      \"type\": \"string\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\"\n    },\n    \"startAt\": {\n      \"type\": \"integer\"\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"isLast\": {\n      \"type\": \"boolean\"\n    },\n    \"values\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-page-bean-project-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: PageBeanProject
---
