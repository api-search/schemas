---
description: ''
layout: schema
name: SuccessfulFeedElementsBatchPost
properties_list:
- description: ''
  name: hasErrors
  type: boolean
- description: ''
  name: results
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-feed-elements-batch-post-schema.json
slug: salesforce-successful-feed-elements-batch-post
source_filename: salesforce-successful-feed-elements-batch-post-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"hasErrors\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"result\": {\n            \"type\": \"object\",\n            \"example\": \"example_value\"\n          },\n          \"statusCode\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          }\n        },\n        \"required\": [\n          \"result\",\n          \"statusCode\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"hasErrors\",\n    \"results\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulFeedElementsBatchPost\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-feed-elements-batch-post-schema.json
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
title: SuccessfulFeedElementsBatchPost
---
