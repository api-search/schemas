---
description: ''
layout: schema
name: Input
properties_list:
- description: ''
  name: richInput
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-input-schema.json
slug: salesforce-input
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"richInput\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"subjectId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"body\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"messageSegments\": {\n              \"type\": \"array\",\n              \"description\": \"\",\n              \"example\": [],\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"text\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"fileId\": {\n                    \"type\": \"string\",\n                    \"example\": \"500123\"\n            \
  \      },\n                  \"altText\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"type\",\n                  \"text\"\n                ]\n              }\n            }\n          },\n          \"required\": [\n            \"messageSegments\"\n          ]\n        },\n        \"capabilities\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"files\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"items\": {\n                  \"type\": \"array\",\n                  \"description\": \"\",\n                  \"example\": [],\n                  \"items\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"id\": {\n                        \"type\": \"object\"\n                      }\n                    },\n \
  \                   \"required\": [\n                      \"id\"\n                    ]\n                  }\n                }\n              },\n              \"required\": [\n                \"items\"\n              ]\n            }\n          },\n          \"required\": [\n            \"files\"\n          ]\n        },\n        \"feedElementType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"subjectId\",\n        \"body\",\n        \"feedElementType\"\n      ]\n    }\n  },\n  \"required\": [\n    \"richInput\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Input\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-input-schema.json
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
title: Input
---
