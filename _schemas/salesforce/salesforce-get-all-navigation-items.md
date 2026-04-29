---
description: ''
layout: schema
name: GetAllNavigationItems
properties_list:
- description: ''
  name: currentPageUrl
  type: string
- description: ''
  name: eTag
  type: string
- description: ''
  name: navItems
  type: array
- description: ''
  name: nextPageUrl
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-get-all-navigation-items-schema.json
slug: salesforce-get-all-navigation-items
source_filename: salesforce-get-all-navigation-items-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentPageUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"eTag\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"navItems\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"availableInClassic\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"availableInLightning\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"color\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"content\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"custom\": {\n            \"type\": \"boolean\",\n      \
  \      \"example\": true\n          },\n          \"developerName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"iconUrl\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"id\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"abc123\"\n          },\n          \"itemType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          },\n          \"objectApiName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"objectLabel\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"objectLabelPlural\": {\n            \"type\": \"string\",\n            \"example\"\
  : \"example_value\"\n          },\n          \"pageReference\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"attributes\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"objectApiName\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"actionName\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"objectApiName\",\n                  \"actionName\"\n                ]\n              },\n              \"state\": {\n                \"type\": \"object\",\n                \"example\": \"example_value\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n       \
  \     \"required\": [\n              \"attributes\",\n              \"state\",\n              \"type\"\n            ]\n          },\n          \"standardType\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"availableInClassic\",\n          \"availableInLightning\",\n          \"color\",\n          \"content\",\n          \"custom\",\n          \"developerName\",\n          \"iconUrl\",\n          \"id\",\n          \"itemType\",\n          \"label\",\n          \"objectApiName\",\n          \"objectLabel\",\n          \"objectLabelPlural\",\n          \"pageReference\",\n          \"standardType\"\n        ]\n      }\n    },\n    \"nextPageUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"currentPageUrl\",\n    \"eTag\",\n    \"navItems\",\n    \"nextPageUrl\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"GetAllNavigationItems\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-get-all-navigation-items-schema.json
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
title: GetAllNavigationItems
---
