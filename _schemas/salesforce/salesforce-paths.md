---
description: ''
layout: schema
name: Paths
properties_list:
- description: ''
  name: /sobjects/Contact
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-paths-schema.json
slug: salesforce-paths
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"/sobjects/Contact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\",\n          \"example\": \"A sample description.\"\n        },\n        \"get\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"responses\": {\n              \"type\": \"object\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"responses\"\n          ]\n        },\n        \"post\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"parameters\": {\n              \"type\": \"array\",\n              \"description\": \"\",\n              \"example\": [],\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"name\": {\n                    \"type\": \"string\",\n                    \"example\":\
  \ \"Example Title\"\n                  },\n                  \"in\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"description\": {\n                    \"type\": \"string\",\n                    \"example\": \"A sample description.\"\n                  },\n                  \"required\": {\n                    \"type\": \"boolean\",\n                    \"example\": true\n                  },\n                  \"schema\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"type\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"type\"\n                    ]\n                  }\n                },\n                \"required\": [\n                  \"name\",\n                  \"in\",\n                  \"description\",\n    \
  \              \"required\",\n                  \"schema\"\n                ]\n              }\n            },\n            \"requestBody\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"content\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"application/json\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"schema\": {\n                          \"type\": \"object\"\n                        }\n                      },\n                      \"required\": [\n                        \"schema\"\n                      ]\n                    }\n                  },\n                  \"required\": [\n                    \"application/json\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"content\"\n              ]\n            },\n            \"responses\": {\n \
  \             \"type\": \"object\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"parameters\",\n            \"requestBody\",\n            \"responses\"\n          ]\n        }\n      },\n      \"required\": [\n        \"description\",\n        \"get\",\n        \"post\"\n      ]\n    }\n  },\n  \"required\": [\n    \"/sobjects/Contact\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Paths\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-paths-schema.json
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
title: Paths
---
