---
description: ''
layout: schema
name: Model1
properties_list:
- description: ''
  name: createdBy
  type: object
- description: ''
  name: createdDate
  type: string
- description: ''
  name: fieldMappingList
  type: array
- description: ''
  name: filters
  type: array
- description: ''
  name: historyUrl
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: isRefreshEnabled
  type: boolean
- description: ''
  name: label
  type: string
- description: ''
  name: lastModifiedBy
  type: object
- description: ''
  name: lastModifiedDate
  type: string
- description: ''
  name: model
  type: object
- description: ''
  name: modelType
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: predictionDefinitionUrl
  type: string
- description: ''
  name: prescribableFields
  type: array
- description: ''
  name: sortOrder
  type: integer
- description: ''
  name: status
  type: string
- description: ''
  name: url
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-model1-schema.json
slug: salesforce-model1
source_filename: salesforce-model1-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdBy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"profilePhotoUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"name\",\n        \"profilePhotoUrl\"\n      ]\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"fieldMappingList\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"modelField\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"label\": {\n \
  \               \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"label\",\n              \"name\",\n              \"type\"\n            ]\n          }\n        },\n        \"required\": [\n          \"modelField\"\n        ]\n      }\n    },\n    \"filters\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"historyUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"isRefreshEnabled\": {\n   \
  \   \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"lastModifiedBy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"profilePhotoUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"name\",\n        \"profilePhotoUrl\"\n      ]\n    },\n    \"lastModifiedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"model\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n       \
  \ \"id\"\n      ]\n    },\n    \"modelType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"predictionDefinitionUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"prescribableFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"customDefinitions\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"field\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"label\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"name\"\
  : {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"label\",\n              \"name\",\n              \"type\"\n            ]\n          }\n        },\n        \"required\": [\n          \"customDefinitions\",\n          \"field\"\n        ]\n      }\n    },\n    \"sortOrder\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"createdBy\",\n    \"createdDate\",\n    \"fieldMappingList\",\n    \"filters\",\n    \"historyUrl\",\n    \"id\",\n    \"isRefreshEnabled\",\n    \"label\",\n    \"lastModifiedBy\",\n\
  \    \"lastModifiedDate\",\n    \"model\",\n    \"modelType\",\n    \"name\",\n    \"predictionDefinitionUrl\",\n    \"prescribableFields\",\n    \"sortOrder\",\n    \"status\",\n    \"url\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Model1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-model1-schema.json
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
title: Model1
---
