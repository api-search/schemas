---
description: A data asset cataloged in the DataZone data catalog.
layout: schema
name: Asset
properties_list:
- description: The unique identifier of the asset
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: domainId
  type: string
- description: ''
  name: owningProjectId
  type: string
- description: ''
  name: typeIdentifier
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: Amazon DataZone
provider_slug: amazon-datazone
schema_file: json-schema/asset-schema.json
slug: asset
source_filename: asset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datazone/json-schema/asset-schema.json\",\n  \"title\": \"Asset\",\n  \"description\": \"A data asset cataloged in the DataZone data catalog.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the asset\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"domainId\": {\n      \"type\": \"string\"\n    },\n    \"owningProjectId\": {\n      \"type\": \"string\"\n    },\n    \"typeIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/json-schema/asset-schema.json
tags:
- AWS
- Data Catalog
- Data Governance
- Data Management
- Data Sharing
- Analytics
title: Asset
---
