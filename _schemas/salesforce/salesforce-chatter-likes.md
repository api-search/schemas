---
description: ''
layout: schema
name: ChatterLikes
properties_list:
- description: ''
  name: isLikedByCurrentUser
  type: boolean
- description: ''
  name: likesMessage
  type: '[''string'', ''null'']'
- description: ''
  name: myLike
  type: '[''string'', ''null'']'
- description: ''
  name: page
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-chatter-likes-schema.json
slug: salesforce-chatter-likes
source_filename: salesforce-chatter-likes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"isLikedByCurrentUser\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"likesMessage\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"myLike\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"page\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"currentPageToken\": {\n          \"type\": \"integer\",\n          \"example\": \"CAUQAA\"\n        },\n        \"currentPageUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"items\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"nextPageToken\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"CAUQAA\"\n  \
  \      },\n        \"nextPageUrl\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"previousPageToken\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"CAUQAA\"\n        },\n        \"previousPageUrl\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"total\": {\n          \"type\": \"integer\",\n          \"example\": 42\n        }\n      },\n      \"required\": [\n        \"currentPageToken\",\n        \"currentPageUrl\",\n        \"items\",\n        \"nextPageToken\",\n        \"nextPageUrl\",\n        \"previousPageToken\",\n        \"previousPageUrl\",\n        \"total\"\n      ]\n    }\n  },\n  \"required\": [\n    \"isLikedByCurrentUser\",\n    \"likesMessage\",\n    \"myLike\",\n    \"page\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatterLikes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-chatter-likes-schema.json
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
title: ChatterLikes
---
