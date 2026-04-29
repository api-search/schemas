---
description: ''
layout: schema
name: SuccessfulNewsFeedElements
properties_list:
- description: ''
  name: currentPageToken
  type: '[''string'', ''null'']'
- description: ''
  name: currentPageUrl
  type: string
- description: ''
  name: elements
  type: array
- description: ''
  name: isModifiedToken
  type: '[''string'', ''null'']'
- description: ''
  name: isModifiedUrl
  type: '[''string'', ''null'']'
- description: ''
  name: nextPageToken
  type: '[''string'', ''null'']'
- description: ''
  name: nextPageUrl
  type: '[''string'', ''null'']'
- description: ''
  name: updatesToken
  type: string
- description: ''
  name: updatesUrl
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-news-feed-elements-schema.json
slug: salesforce-successful-news-feed-elements
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentPageToken\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"CAUQAA\"\n    },\n    \"currentPageUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"elements\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"isModifiedToken\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"CAUQAA\"\n    },\n    \"isModifiedUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"CAUQAA\"\n    },\n    \"nextPageUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"updatesToken\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n\
  \    \"updatesUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"currentPageToken\",\n    \"currentPageUrl\",\n    \"elements\",\n    \"isModifiedToken\",\n    \"isModifiedUrl\",\n    \"nextPageToken\",\n    \"nextPageUrl\",\n    \"updatesToken\",\n    \"updatesUrl\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulNewsFeedElements\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-news-feed-elements-schema.json
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
title: SuccessfulNewsFeedElements
---
