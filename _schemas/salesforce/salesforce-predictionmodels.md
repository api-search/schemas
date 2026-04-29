---
description: ''
layout: schema
name: Predictionmodels
properties_list:
- description: ''
  name: models
  type: array
- description: ''
  name: totalSize
  type: integer
- description: ''
  name: url
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-predictionmodels-schema.json
slug: salesforce-predictionmodels
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"models\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"createdBy\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              },\n              \"profilePhotoUrl\": {\n                \"type\": \"string\",\n                \"example\": \"https://www.example.com\"\n              }\n            },\n            \"required\": [\n              \"id\",\n              \"name\",\n              \"profilePhotoUrl\"\n            ]\n          },\n          \"createdDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\
  \n          },\n          \"fieldMappingList\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"modelField\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"label\": {\n                      \"type\": \"object\"\n                    },\n                    \"name\": {\n                      \"type\": \"object\"\n                    },\n                    \"type\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"label\",\n                    \"name\",\n                    \"type\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"modelField\"\n              ]\n            }\n          },\n          \"filters\"\
  : {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"historyUrl\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"isRefreshEnabled\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"lastModifiedBy\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\
  \n              },\n              \"profilePhotoUrl\": {\n                \"type\": \"string\",\n                \"example\": \"https://www.example.com\"\n              }\n            },\n            \"required\": [\n              \"id\",\n              \"name\",\n              \"profilePhotoUrl\"\n            ]\n          },\n          \"lastModifiedDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"model\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              }\n            },\n            \"required\": [\n              \"id\"\n            ]\n          },\n          \"modelType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n\
  \          \"predictionDefinitionUrl\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"prescribableFields\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"customDefinitions\": {\n                  \"type\": \"array\",\n                  \"description\": \"\",\n                  \"example\": [],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                },\n                \"field\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"label\": {\n                      \"type\": \"object\"\n                    },\n                    \"name\": {\n                      \"type\": \"object\"\n                    },\n                    \"type\": {\n \
  \                     \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"label\",\n                    \"name\",\n                    \"type\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"customDefinitions\",\n                \"field\"\n              ]\n            }\n          },\n          \"sortOrder\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          }\n        },\n        \"required\": [\n          \"createdBy\",\n          \"createdDate\",\n          \"fieldMappingList\",\n          \"filters\",\n          \"historyUrl\",\n          \"id\",\n          \"isRefreshEnabled\",\n    \
  \      \"label\",\n          \"lastModifiedBy\",\n          \"lastModifiedDate\",\n          \"model\",\n          \"modelType\",\n          \"name\",\n          \"predictionDefinitionUrl\",\n          \"prescribableFields\",\n          \"sortOrder\",\n          \"status\",\n          \"url\"\n        ]\n      }\n    },\n    \"totalSize\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"models\",\n    \"totalSize\",\n    \"url\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Predictionmodels\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-predictionmodels-schema.json
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
title: Predictionmodels
---
