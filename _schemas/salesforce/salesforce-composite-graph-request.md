---
description: ''
layout: schema
name: CompositeGraphRequest
properties_list:
- description: ''
  name: graphs
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-composite-graph-request-schema.json
slug: salesforce-composite-graph-request
source_filename: salesforce-composite-graph-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"graphs\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"graphId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"compositeRequest\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"method\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"url\": {\n                  \"type\": \"string\",\n                  \"example\": \"https://www.example.com\"\n                },\n                \"referenceId\": {\n                  \"type\": \"string\",\n                  \"example\": \"500123\"\n     \
  \           },\n                \"body\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"Name\": {\n                      \"type\": \"object\"\n                    },\n                    \"Custom__c\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"Name\",\n                    \"Custom__c\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"method\",\n                \"url\",\n                \"referenceId\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"graphId\",\n          \"compositeRequest\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"graphs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompositeGraphRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-composite-graph-request-schema.json
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
title: CompositeGraphRequest
---
