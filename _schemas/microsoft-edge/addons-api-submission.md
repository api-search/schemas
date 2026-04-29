---
description: An extension submission for review and publishing in the Microsoft Edge Add-ons store
layout: schema
name: Submission
properties_list:
- description: Submission identifier
  name: id
  type: string
- description: Parent product identifier
  name: productId
  type: string
- description: Submission status
  name: status
  type: string
- description: Submission creation timestamp
  name: createdUtc
  type: string
- description: Submission completion timestamp
  name: completedUtc
  type: string
provider_name: Microsoft Edge
provider_slug: microsoft-edge
schema_file: json-schema/addons-api-submission-schema.json
slug: addons-api-submission
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/addons-api-submission-schema.json\",\n  \"title\": \"Submission\",\n  \"description\": \"An extension submission for review and publishing in the Microsoft Edge Add-ons store\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Submission identifier\"\n    },\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent product identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Submission status\",\n      \"enum\": [\"Draft\", \"InReview\", \"Published\", \"Failed\", \"Cancelled\"]\n    },\n    \"createdUtc\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Submission creation timestamp\"\n    },\n    \"completedUtc\": {\n      \"\
  type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Submission completion timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/json-schema/addons-api-submission-schema.json
tags:
- Browser
- Chromium
- Developer Tools
- Edge
- Extensions
- Microsoft
- Progressive Web Apps
- Web Development
- WebView
title: Submission
---
