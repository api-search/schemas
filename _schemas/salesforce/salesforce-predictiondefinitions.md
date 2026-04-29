---
description: ''
layout: schema
name: Predictiondefinitions
properties_list:
- description: ''
  name: nextPageUrl
  type: '[''string'', ''null'']'
- description: ''
  name: predictionDefinitions
  type: array
- description: ''
  name: totalSize
  type: integer
- description: ''
  name: url
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-predictiondefinitions-schema.json
slug: salesforce-predictiondefinitions
source_filename: salesforce-predictiondefinitions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextPageUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"predictionDefinitions\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"countOfActiveModels\": {\n            \"type\": \"integer\",\n            \"example\": 42\n          },\n          \"countOfModels\": {\n            \"type\": \"integer\",\n            \"example\": 42\n          },\n          \"createdBy\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"profilePhotoUrl\": {\n        \
  \        \"type\": \"string\",\n                \"example\": \"https://www.example.com\"\n              }\n            },\n            \"required\": [\n              \"id\",\n              \"name\",\n              \"profilePhotoUrl\"\n            ]\n          },\n          \"createdDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"lastModifiedBy\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"profilePhotoUrl\":\
  \ {\n                \"type\": \"string\",\n                \"example\": \"https://www.example.com\"\n              }\n            },\n            \"required\": [\n              \"id\",\n              \"name\",\n              \"profilePhotoUrl\"\n            ]\n          },\n          \"lastModifiedDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"modelsUrl\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"outcome\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"goal\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"label\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n         \
  \     },\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              }\n            },\n            \"required\": [\n              \"goal\",\n              \"label\",\n              \"name\"\n            ]\n          },\n          \"predictionType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          }\n        },\n        \"required\": [\n          \"countOfActiveModels\",\n          \"countOfModels\",\n          \"createdBy\",\n          \"createdDate\",\n          \"id\",\n          \"label\",\n          \"lastModifiedBy\",\n          \"lastModifiedDate\",\n          \"modelsUrl\",\n          \"name\",\n          \"outcome\",\n        \
  \  \"predictionType\",\n          \"status\",\n          \"url\"\n        ]\n      }\n    },\n    \"totalSize\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"nextPageUrl\",\n    \"predictionDefinitions\",\n    \"totalSize\",\n    \"url\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Predictiondefinitions\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-predictiondefinitions-schema.json
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
title: Predictiondefinitions
---
