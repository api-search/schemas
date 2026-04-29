---
description: An asset within a data set revision, representing an individual piece of data.
layout: schema
name: Asset
properties_list:
- description: ''
  name: Id
  type: string
- description: ''
  name: Arn
  type: string
- description: ''
  name: DataSetId
  type: string
- description: ''
  name: RevisionId
  type: string
- description: ''
  name: Name
  type: string
- description: ''
  name: AssetType
  type: string
- description: ''
  name: AssetDetails
  type: object
- description: ''
  name: CreatedAt
  type: string
- description: ''
  name: UpdatedAt
  type: string
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/asset-schema.json
slug: asset
source_filename: asset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/asset-schema.json\",\n  \"title\": \"Asset\",\n  \"description\": \"An asset within a data set revision, representing an individual piece of data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\"\n    },\n    \"Arn\": {\n      \"type\": \"string\"\n    },\n    \"DataSetId\": {\n      \"type\": \"string\"\n    },\n    \"RevisionId\": {\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"AssetType\": {\n      \"type\": \"string\"\n    },\n    \"AssetDetails\": {\n      \"type\": \"object\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/asset-schema.json
tags:
- AWS
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: Asset
---
