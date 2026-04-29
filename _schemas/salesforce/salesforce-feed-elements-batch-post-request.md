---
description: ''
layout: schema
name: FeedElementsBatchPostRequest
properties_list:
- description: ''
  name: inputs
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-feed-elements-batch-post-request-schema.json
slug: salesforce-feed-elements-batch-post-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"richInput\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"subjectId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"body\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"messageSegments\": {\n                    \"type\": \"array\",\n                    \"description\": \"\",\n                    \"example\": [],\n                    \"items\": {\n                      \"type\": \"object\"\n                    }\n                  }\n                },\n                \"required\": [\n                  \"messageSegments\"\n                ]\n              },\n              \"capabilities\"\
  : {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"files\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"items\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"items\"\n                    ]\n                  }\n                },\n                \"required\": [\n                  \"files\"\n                ]\n              },\n              \"feedElementType\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"subjectId\",\n              \"body\",\n              \"feedElementType\"\n            ]\n          }\n        },\n        \"required\": [\n          \"richInput\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ],\n \
  \ \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FeedElementsBatchPostRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-feed-elements-batch-post-request-schema.json
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
title: FeedElementsBatchPostRequest
---
