---
description: ''
layout: schema
name: App
properties_list:
- description: The unique ID of the Amplify app.
  name: appId
  type: string
- description: The Amazon Resource Name (ARN) of the Amplify app.
  name: appArn
  type: string
- description: The name of the Amplify app.
  name: name
  type: string
- description: The description of the Amplify app.
  name: description
  type: string
- description: The Git repository for the Amplify app.
  name: repository
  type: string
- description: ''
  name: platform
  type: string
- description: ''
  name: createTime
  type: string
- description: ''
  name: updateTime
  type: string
- description: ''
  name: defaultDomain
  type: string
- description: ''
  name: productionBranch
  type: object
provider_name: Amazon Amplify
provider_slug: amazon-amplify
schema_file: json-schema/amazon-amplify-app-schema.json
slug: amazon-amplify-app
source_filename: amazon-amplify-app-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"App\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID of the Amplify app.\"\n    },\n    \"appArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the Amplify app.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Amplify app.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the Amplify app.\"\n    },\n    \"repository\": {\n      \"type\": \"string\",\n      \"description\": \"The Git repository for the Amplify app.\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"WEB\",\n        \"WEB_DYNAMIC\",\n        \"WEB_COMPUTE\"\n      ]\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n\
  \    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"defaultDomain\": {\n      \"type\": \"string\"\n    },\n    \"productionBranch\": {\n      \"$ref\": \"#/definitions/ProductionBranch\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-amplify/refs/heads/main/json-schema/amazon-amplify-app-schema.json
tags:
- Frontend
- Full Stack
- Hosting
- Mobile Development
- Web Applications
title: App
---
