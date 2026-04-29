---
description: Specification for creating or updating an asset
layout: schema
name: AssetDefinition
properties_list:
- description: Display name of the asset
  name: name
  type: string
- description: Description of the asset
  name: description
  type: string
- description: Customer-defined unique key
  name: customerKey
  type: string
- description: ''
  name: category
  type: object
- description: Primary content of the asset
  name: content
  type: string
- description: Channel-specific content views
  name: views
  type: object
- description: Asset-type-specific data
  name: data
  type: object
- description: ''
  name: tags
  type: array
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-asset-definition-schema.json
slug: salesforce-marketing-cloud-asset-definition
source_filename: salesforce-marketing-cloud-asset-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssetDefinition\",\n  \"type\": \"object\",\n  \"description\": \"Specification for creating or updating an asset\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the asset\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the asset\"\n    },\n    \"customerKey\": {\n      \"type\": \"string\",\n      \"description\": \"Customer-defined unique key\"\n    },\n    \"category\": {\n      \"type\": \"object\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Primary content of the asset\"\n    },\n    \"views\": {\n      \"type\": \"object\",\n      \"description\": \"Channel-specific content views\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Asset-type-specific data\"\n    },\n    \"tags\": {\n      \"type\": \"\
  array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-asset-definition-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: AssetDefinition
---
