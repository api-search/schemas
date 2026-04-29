---
description: Represents a marketing asset in Content Builder. Assets include emails, templates, images, content blocks, and other content types used in marketing campaigns.
layout: schema
name: Asset
properties_list:
- description: System-generated unique identifier for the asset
  name: id
  type: integer
- description: Customer-defined unique key for the asset
  name: customerKey
  type: string
- description: Display name of the asset
  name: name
  type: string
- description: Description of the asset
  name: description
  type: string
- description: Category (folder) containing the asset
  name: category
  type: object
- description: Primary content of the asset, typically HTML or text depending on asset type
  name: content
  type: string
- description: Channel-specific content views (e.g., html, text, subjectLine, preheader)
  name: views
  type: object
- description: Asset-type-specific data and configuration
  name: data
  type: object
- description: Tags assigned to the asset for organization
  name: tags
  type: array
- description: ''
  name: status
  type: object
- description: ''
  name: createdDate
  type: string
- description: ''
  name: modifiedDate
  type: string
- description: ''
  name: createdBy
  type: object
- description: ''
  name: modifiedBy
  type: object
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-asset-schema.json
slug: salesforce-marketing-cloud-asset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Asset\",\n  \"type\": \"object\",\n  \"description\": \"Represents a marketing asset in Content Builder. Assets include emails, templates, images, content blocks, and other content types used in marketing campaigns.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"System-generated unique identifier for the asset\"\n    },\n    \"customerKey\": {\n      \"type\": \"string\",\n      \"description\": \"Customer-defined unique key for the asset\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the asset\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the asset\"\n    },\n    \"category\": {\n      \"type\": \"object\",\n      \"description\": \"Category (folder) containing the asset\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"Primary content of the asset, typically HTML or text depending on asset type\"\n    },\n    \"views\": {\n      \"type\": \"object\",\n      \"description\": \"Channel-specific content views (e.g., html, text, subjectLine, preheader)\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Asset-type-specific data and configuration\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags assigned to the asset for organization\"\n    },\n    \"status\": {\n      \"type\": \"object\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\"\n    },\n    \"createdBy\": {\n      \"type\": \"object\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-asset-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: Asset
---
