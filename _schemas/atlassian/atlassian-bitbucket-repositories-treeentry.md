---
description: Base type for most resource objects. It defines the common `type` element that identifies an object's type. It also identifies the element as Swagger's `discriminator`.
layout: schema
name: treeentry
properties_list:
- description: ''
  name: type
  type: string
- description: The path in the repository
  name: path
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-repositories-treeentry-schema.json
slug: atlassian-bitbucket-repositories-treeentry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"treeentry\",\n  \"type\": \"object\",\n  \"description\": \"Base type for most resource objects. It defines the common `type` element that identifies an object's type. It also identifies the element as Swagger's `discriminator`.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The path in the repository\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-repositories-treeentry-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: treeentry
---
