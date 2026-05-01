---
description: Request body for creating a DataZone project.
layout: schema
name: Create Project Request
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
provider_name: Amazon DataZone
provider_slug: amazon-datazone
schema_file: json-schema/create-project-request-schema.json
slug: create-project-request
source_filename: create-project-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datazone/json-schema/create-project-request-schema.json\",\n  \"title\": \"Create Project Request\",\n  \"description\": \"Request body for creating a DataZone project.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/json-schema/create-project-request-schema.json
tags:
- Data Catalog
- Data Governance
- Data Management
- Data Sharing
- Analytics
title: Create Project Request
---
