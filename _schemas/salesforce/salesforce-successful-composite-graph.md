---
description: ''
layout: schema
name: SuccessfulCompositeGraph
properties_list:
- description: ''
  name: graphs
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-composite-graph-schema.json
slug: salesforce-successful-composite-graph
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"graphs\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"graphId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"graphResponse\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"compositeResponse\": {\n                \"type\": \"array\",\n                \"description\": \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"body\": {\n                      \"type\": \"object\"\n                    },\n                    \"httpHeaders\": {\n                      \"type\": \"object\"\n                    },\n                    \"httpStatusCode\": {\n                      \"type\": \"object\"\
  \n                    },\n                    \"referenceId\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"body\",\n                    \"httpHeaders\",\n                    \"httpStatusCode\",\n                    \"referenceId\"\n                  ]\n                }\n              }\n            },\n            \"required\": [\n              \"compositeResponse\"\n            ]\n          },\n          \"isSuccessful\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          }\n        },\n        \"required\": [\n          \"graphId\",\n          \"graphResponse\",\n          \"isSuccessful\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"graphs\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulCompositeGraph\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-composite-graph-schema.json
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
title: SuccessfulCompositeGraph
---
