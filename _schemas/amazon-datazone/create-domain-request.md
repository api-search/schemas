---
description: Request body for creating a DataZone domain.
layout: schema
name: Create Domain Request
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: domainExecutionRole
  type: string
- description: ''
  name: tags
  type: object
provider_name: Amazon DataZone
provider_slug: amazon-datazone
schema_file: json-schema/create-domain-request-schema.json
slug: create-domain-request
source_filename: create-domain-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datazone/json-schema/create-domain-request-schema.json\",\n  \"title\": \"Create Domain Request\",\n  \"description\": \"Request body for creating a DataZone domain.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"domainExecutionRole\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"domainExecutionRole\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/json-schema/create-domain-request-schema.json
tags:
- AWS
- Data Catalog
- Data Governance
- Data Management
- Data Sharing
- Analytics
title: Create Domain Request
---
