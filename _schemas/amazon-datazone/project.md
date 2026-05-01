---
description: A DataZone project that serves as a container for data assets and environments.
layout: schema
name: Project
properties_list:
- description: The unique identifier of the project
  name: id
  type: string
- description: ''
  name: domainId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: Amazon DataZone
provider_slug: amazon-datazone
schema_file: json-schema/project-schema.json
slug: project
source_filename: project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datazone/json-schema/project-schema.json\",\n  \"title\": \"Project\",\n  \"description\": \"A DataZone project that serves as a container for data assets and environments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the project\"\n    },\n    \"domainId\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/json-schema/project-schema.json
tags:
- Data Catalog
- Data Governance
- Data Management
- Data Sharing
- Analytics
title: Project
---
