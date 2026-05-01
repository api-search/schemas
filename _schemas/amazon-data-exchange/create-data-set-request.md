---
description: Request body for creating a new data set.
layout: schema
name: Create Data Set Request
properties_list:
- description: ''
  name: Name
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: AssetType
  type: string
- description: ''
  name: Tags
  type: object
provider_name: Amazon Data Exchange
provider_slug: amazon-data-exchange
schema_file: json-schema/create-data-set-request-schema.json
slug: create-data-set-request
source_filename: create-data-set-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-exchange/json-schema/create-data-set-request-schema.json\",\n  \"title\": \"Create Data Set Request\",\n  \"description\": \"Request body for creating a new data set.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"Name\",\n    \"Description\",\n    \"AssetType\"\n  ],\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"AssetType\": {\n      \"type\": \"string\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-exchange/refs/heads/main/json-schema/create-data-set-request-schema.json
tags:
- Data Exchange
- Data Marketplace
- Third-Party Data
- Analytics
- Subscriptions
title: Create Data Set Request
---
