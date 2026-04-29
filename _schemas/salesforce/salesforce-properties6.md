---
description: ''
layout: schema
name: Properties6
properties_list:
- description: ''
  name: message
  type: object
- description: ''
  name: errorCode
  type: object
- description: ''
  name: fields
  type: object
- description: ''
  name: extendedErrorDetails
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-properties6-schema.json
slug: salesforce-properties6
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"type\"\n      ]\n    },\n    \"errorCode\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"type\"\n      ]\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"items\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n         \
  \   \"type\"\n          ]\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"items\"\n      ]\n    },\n    \"extendedErrorDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"items\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"properties\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"extendedErrorCode\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"type\": {\n                      \"type\": \"string\",\n                      \"example\": \"example_value\"\n                    }\n                  },\n                  \"required\": [\n                    \"type\"\n       \
  \           ]\n                }\n              },\n              \"required\": [\n                \"extendedErrorCode\"\n              ]\n            }\n          },\n          \"required\": [\n            \"type\",\n            \"properties\"\n          ]\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"items\"\n      ]\n    }\n  },\n  \"required\": [\n    \"message\",\n    \"errorCode\",\n    \"fields\",\n    \"extendedErrorDetails\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Properties6\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-properties6-schema.json
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
title: Properties6
---
