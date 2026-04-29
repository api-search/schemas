---
description: ''
layout: schema
name: AccountswithCursorsPagination
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: errors
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-accountswith-cursors-pagination-schema.json
slug: salesforce-accountswith-cursors-pagination
source_filename: salesforce-accountswith-cursors-pagination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"uiapi\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"query\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Account\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"edges\": {\n                      \"type\": \"array\",\n                      \"description\": \"\",\n                      \"example\": [],\n                      \"items\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"totalCount\": {\n                      \"type\": \"integer\",\n                      \"example\": 42\n                    },\n                    \"pageInfo\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n           \
  \             \"hasNextPage\": {\n                          \"type\": \"object\"\n                        },\n                        \"hasPreviousPage\": {\n                          \"type\": \"object\"\n                        },\n                        \"startCursor\": {\n                          \"type\": \"object\"\n                        },\n                        \"endCursor\": {\n                          \"type\": \"object\"\n                        }\n                      },\n                      \"required\": [\n                        \"hasNextPage\",\n                        \"hasPreviousPage\",\n                        \"startCursor\",\n                        \"endCursor\"\n                      ]\n                    }\n                  },\n                  \"required\": [\n                    \"edges\",\n                    \"totalCount\",\n                    \"pageInfo\"\n                  ]\n                }\n              },\n              \"required\": [\n\
  \                \"Account\"\n              ]\n            }\n          },\n          \"required\": [\n            \"query\"\n          ]\n        }\n      },\n      \"required\": [\n        \"uiapi\"\n      ]\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"data\",\n    \"errors\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountswithCursorsPagination\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-accountswith-cursors-pagination-schema.json
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
title: AccountswithCursorsPagination
---
