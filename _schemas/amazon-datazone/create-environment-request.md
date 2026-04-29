---
description: Request body for creating a DataZone environment.
layout: schema
name: Create Environment Request
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: domainIdentifier
  type: string
- description: ''
  name: projectIdentifier
  type: string
- description: ''
  name: environmentProfileIdentifier
  type: string
provider_name: Amazon DataZone
provider_slug: amazon-datazone
schema_file: json-schema/create-environment-request-schema.json
slug: create-environment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datazone/json-schema/create-environment-request-schema.json\",\n  \"title\": \"Create Environment Request\",\n  \"description\": \"Request body for creating a DataZone environment.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"domainIdentifier\",\n    \"projectIdentifier\",\n    \"environmentProfileIdentifier\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"domainIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"projectIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"environmentProfileIdentifier\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/json-schema/create-environment-request-schema.json
tags:
- AWS
- Data Catalog
- Data Governance
- Data Management
- Data Sharing
- Analytics
title: Create Environment Request
---
