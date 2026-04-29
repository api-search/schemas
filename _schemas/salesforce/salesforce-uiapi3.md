---
description: ''
layout: schema
name: Uiapi3
properties_list:
- description: ''
  name: query
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-uiapi3-schema.json
slug: salesforce-uiapi3
source_filename: salesforce-uiapi3-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Account\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"edges\": {\n              \"type\": \"array\",\n              \"description\": \"\",\n              \"example\": [],\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"node\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"Id\": {\n                        \"type\": \"object\"\n                      },\n                      \"Name\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"Id\",\n                      \"Name\"\n                    ]\n                  }\n                },\n                \"required\": [\n \
  \                 \"node\"\n                ]\n              }\n            },\n            \"totalCount\": {\n              \"type\": \"integer\",\n              \"example\": 42\n            },\n            \"pageInfo\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"hasNextPage\": {\n                  \"type\": \"boolean\",\n                  \"example\": true\n                },\n                \"hasPreviousPage\": {\n                  \"type\": \"boolean\",\n                  \"example\": true\n                },\n                \"startCursor\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"endCursor\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                }\n              },\n              \"required\": [\n                \"hasNextPage\",\n                \"hasPreviousPage\",\n                \"\
  startCursor\",\n                \"endCursor\"\n              ]\n            }\n          },\n          \"required\": [\n            \"edges\",\n            \"totalCount\",\n            \"pageInfo\"\n          ]\n        }\n      },\n      \"required\": [\n        \"Account\"\n      ]\n    }\n  },\n  \"required\": [\n    \"query\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Uiapi3\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-uiapi3-schema.json
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
title: Uiapi3
---
