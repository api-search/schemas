---
description: ''
layout: schema
name: FeedElementsPostandSearchRequest
properties_list:
- description: ''
  name: body
  type: object
- description: ''
  name: capabilities
  type: object
- description: ''
  name: subjectId
  type: string
- description: ''
  name: feedElementType
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-feed-elements-postand-search-request-schema.json
slug: salesforce-feed-elements-postand-search-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"messageSegments\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"text\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"markupType\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              }\n            },\n            \"required\": [\n              \"type\"\n            ]\n          }\n        }\n      },\n      \"required\"\
  : [\n        \"messageSegments\"\n      ]\n    },\n    \"capabilities\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"files\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"items\": {\n              \"type\": \"array\",\n              \"description\": \"\",\n              \"example\": [],\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"example\": \"abc123\"\n                  }\n                },\n                \"required\": [\n                  \"id\"\n                ]\n              }\n            }\n          },\n          \"required\": [\n            \"items\"\n          ]\n        }\n      },\n      \"required\": [\n        \"files\"\n      ]\n    },\n    \"subjectId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"feedElementType\": {\n      \"\
  type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"body\",\n    \"capabilities\",\n    \"subjectId\",\n    \"feedElementType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FeedElementsPostandSearchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-feed-elements-postand-search-request-schema.json
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
title: FeedElementsPostandSearchRequest
---
