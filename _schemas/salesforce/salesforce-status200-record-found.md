---
description: ''
layout: schema
name: Status200-RecordFound
properties_list:
- description: ''
  name: apiName
  type: string
- description: ''
  name: contextDefinitions
  type: array
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: usageType
  type: string
- description: ''
  name: versions
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-status200-record-found-schema.json
slug: salesforce-status200-record-found
source_filename: salesforce-status200-record-found-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"contextDefinitions\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"usageType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"apiName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"\
  A sample description.\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"rank\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"showExplExternally\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"startDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"steps\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"actionType\": {\n                  \"type\": \"string\"\
  ,\n                  \"example\": \"example_value\"\n                },\n                \"assignment\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"assignedParameter\": {\n                      \"type\": \"object\"\n                    },\n                    \"expression\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"assignedParameter\",\n                    \"expression\"\n                  ]\n                },\n                \"description\": {\n                  \"type\": \"string\",\n                  \"example\": \"A sample description.\"\n                },\n                \"name\": {\n                  \"type\": \"string\",\n                  \"example\": \"Example Title\"\n                },\n                \"resultIncluded\": {\n                  \"type\": \"boolean\",\n                  \"example\": true\n  \
  \              },\n                \"sequenceNumber\": {\n                  \"type\": \"integer\",\n                  \"example\": 10\n                },\n                \"shouldExposeConditionDetails\": {\n                  \"type\": \"boolean\",\n                  \"example\": true\n                },\n                \"shouldExposeExecPathMsgOnly\": {\n                  \"type\": \"boolean\",\n                  \"example\": true\n                },\n                \"shouldShowExplExternally\": {\n                  \"type\": \"boolean\",\n                  \"example\": true\n                },\n                \"stepType\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                }\n              },\n              \"required\": [\n                \"actionType\",\n                \"assignment\",\n                \"description\",\n                \"name\",\n                \"resultIncluded\",\n                \"sequenceNumber\",\n\
  \                \"shouldExposeConditionDetails\",\n                \"shouldExposeExecPathMsgOnly\",\n                \"shouldShowExplExternally\",\n                \"stepType\"\n              ]\n            }\n          },\n          \"variables\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"collection\": {\n                  \"type\": \"boolean\",\n                  \"example\": true\n                },\n                \"dataType\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"description\": {\n                  \"type\": \"string\",\n                  \"example\": \"A sample description.\"\n                },\n                \"input\": {\n                  \"type\": \"boolean\",\n                  \"example\": true\n        \
  \        },\n                \"name\": {\n                  \"type\": \"string\",\n                  \"example\": \"Example Title\"\n                },\n                \"output\": {\n                  \"type\": \"boolean\",\n                  \"example\": true\n                },\n                \"type\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"value\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                }\n              },\n              \"required\": [\n                \"collection\",\n                \"dataType\",\n                \"description\",\n                \"input\",\n                \"name\",\n                \"output\",\n                \"type\",\n                \"value\"\n              ]\n            }\n          },\n          \"versionNumber\": {\n            \"type\": \"integer\",\n            \"example\": 10\n        \
  \  }\n        },\n        \"required\": [\n          \"apiName\",\n          \"description\",\n          \"enabled\",\n          \"id\",\n          \"name\",\n          \"rank\",\n          \"showExplExternally\",\n          \"startDate\",\n          \"steps\",\n          \"variables\",\n          \"versionNumber\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"apiName\",\n    \"contextDefinitions\",\n    \"id\",\n    \"name\",\n    \"usageType\",\n    \"versions\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status200-RecordFound\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-status200-record-found-schema.json
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
title: Status200-RecordFound
---
