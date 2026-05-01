---
description: ''
layout: schema
name: Branch
properties_list:
- description: ''
  name: branchName
  type: string
- description: ''
  name: branchArn
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: stage
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: activeJobId
  type: string
provider_name: Amazon Amplify
provider_slug: amazon-amplify
schema_file: json-schema/amazon-amplify-branch-schema.json
slug: amazon-amplify-branch
source_filename: amazon-amplify-branch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Branch\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branchName\": {\n      \"type\": \"string\"\n    },\n    \"branchArn\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"stage\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PRODUCTION\",\n        \"BETA\",\n        \"DEVELOPMENT\",\n        \"EXPERIMENTAL\",\n        \"PULL_REQUEST\"\n      ]\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"activeJobId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-amplify/refs/heads/main/json-schema/amazon-amplify-branch-schema.json
tags:
- Frontend
- Full Stack
- Hosting
- Mobile Development
- Web Applications
title: Branch
---
