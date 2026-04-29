---
description: ''
layout: schema
name: CreateRepoRequest
properties_list:
- description: Repository name
  name: name
  type: string
- description: Repository type
  name: type
  type: string
- description: Organization to create the repo under
  name: organization
  type: string
- description: Whether the repo should be private
  name: private
  type: boolean
- description: SDK for Spaces (required when type is space)
  name: sdk
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-hub-create-repo-request-schema.json
slug: hugging-face-hub-create-repo-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateRepoRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Repository name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Repository type\"\n    },\n    \"organization\": {\n      \"type\": \"string\",\n      \"description\": \"Organization to create the repo under\"\n    },\n    \"private\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repo should be private\"\n    },\n    \"sdk\": {\n      \"type\": \"string\",\n      \"description\": \"SDK for Spaces (required when type is space)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-hub-create-repo-request-schema.json
tags: []
title: CreateRepoRequest
---
