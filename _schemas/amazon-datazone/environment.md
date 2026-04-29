---
description: A DataZone environment that provides data access capabilities for a project.
layout: schema
name: Environment
properties_list:
- description: The unique identifier of the environment
  name: id
  type: string
- description: ''
  name: domainId
  type: string
- description: ''
  name: projectId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: Amazon DataZone
provider_slug: amazon-datazone
schema_file: json-schema/environment-schema.json
slug: environment
source_filename: environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datazone/json-schema/environment-schema.json\",\n  \"title\": \"Environment\",\n  \"description\": \"A DataZone environment that provides data access capabilities for a project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the environment\"\n    },\n    \"domainId\": {\n      \"type\": \"string\"\n    },\n    \"projectId\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"CREATING\",\n        \"DELETED\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/json-schema/environment-schema.json
tags:
- AWS
- Data Catalog
- Data Governance
- Data Management
- Data Sharing
- Analytics
title: Environment
---
