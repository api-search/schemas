---
description: Base type for most resource objects. It defines the common `type` element that identifies an object's type. It also identifies the element as Swagger's `discriminator`.
layout: schema
name: error
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: error
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-user-error-schema.json
slug: atlassian-bitbucket-user-error
source_filename: atlassian-bitbucket-user-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"error\",\n  \"type\": \"object\",\n  \"description\": \"Base type for most resource objects. It defines the common `type` element that identifies an object's type. It also identifies the element as Swagger's `discriminator`.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"error\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-user-error-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: error
---
