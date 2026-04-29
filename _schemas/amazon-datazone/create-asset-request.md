---
description: Request body for creating a data asset.
layout: schema
name: Create Asset Request
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
  name: owningProjectIdentifier
  type: string
- description: ''
  name: typeIdentifier
  type: string
provider_name: Amazon DataZone
provider_slug: amazon-datazone
schema_file: json-schema/create-asset-request-schema.json
slug: create-asset-request
source_filename: create-asset-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datazone/json-schema/create-asset-request-schema.json\",\n  \"title\": \"Create Asset Request\",\n  \"description\": \"Request body for creating a data asset.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"domainIdentifier\",\n    \"owningProjectIdentifier\",\n    \"typeIdentifier\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"domainIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"owningProjectIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"typeIdentifier\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/json-schema/create-asset-request-schema.json
tags:
- AWS
- Data Catalog
- Data Governance
- Data Management
- Data Sharing
- Analytics
title: Create Asset Request
---
