---
description: ''
layout: schema
name: Getchannelmember
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: Id
  type: string
- description: ''
  name: IsDeleted
  type: boolean
- description: ''
  name: DeveloperName
  type: string
- description: ''
  name: Language
  type: string
- description: ''
  name: MasterLabel
  type: string
- description: ''
  name: NamespacePrefix
  type: '[''string'', ''null'']'
- description: ''
  name: ManageableState
  type: string
- description: ''
  name: CreatedDate
  type: string
- description: ''
  name: CreatedById
  type: string
- description: ''
  name: LastModifiedDate
  type: string
- description: ''
  name: LastModifiedById
  type: string
- description: ''
  name: SystemModstamp
  type: string
- description: ''
  name: FullName
  type: string
- description: ''
  name: Metadata
  type: object
- description: ''
  name: EventChannel
  type: string
- description: ''
  name: SelectedEntity
  type: string
- description: ''
  name: FilterExpression
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-getchannelmember-schema.json
slug: salesforce-getchannelmember
source_filename: salesforce-getchannelmember-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"url\"\n      ]\n    },\n    \"Id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"IsDeleted\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"DeveloperName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Language\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"MasterLabel\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"NamespacePrefix\": {\n      \"type\": \"['string', 'null']\",\n      \"example\":\
  \ \"example_value\"\n    },\n    \"ManageableState\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"SystemModstamp\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"FullName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"enrichedFields\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n      \
  \  },\n        \"eventChannel\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"filterExpression\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"selectedEntity\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"urls\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"enrichedFields\",\n        \"eventChannel\",\n        \"filterExpression\",\n        \"selectedEntity\",\n        \"urls\"\n      ]\n    },\n    \"EventChannel\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"SelectedEntity\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"FilterExpression\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n   \
  \ }\n  },\n  \"required\": [\n    \"attributes\",\n    \"Id\",\n    \"IsDeleted\",\n    \"DeveloperName\",\n    \"Language\",\n    \"MasterLabel\",\n    \"NamespacePrefix\",\n    \"ManageableState\",\n    \"CreatedDate\",\n    \"CreatedById\",\n    \"LastModifiedDate\",\n    \"LastModifiedById\",\n    \"SystemModstamp\",\n    \"FullName\",\n    \"Metadata\",\n    \"EventChannel\",\n    \"SelectedEntity\",\n    \"FilterExpression\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Getchannelmember\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-getchannelmember-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: Getchannelmember
---
