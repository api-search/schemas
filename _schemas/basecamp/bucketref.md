---
description: Reference to the project (bucket) that contains a resource
layout: schema
name: BucketRef
properties_list:
- description: Project ID
  name: id
  type: integer
- description: Project name
  name: name
  type: string
- description: Resource type, always "Project"
  name: type
  type: string
- description: API URL for the project
  name: url
  type: string
- description: Web URL for the project
  name: app_url
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/bucketref-schema.json
slug: bucketref
source_filename: bucketref-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/bucketref-schema.json\",\n  \"title\": \"BucketRef\",\n  \"type\": \"object\",\n  \"description\": \"Reference to the project (bucket) that contains a resource\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Project ID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Project name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type, always \\\"Project\\\"\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL for the project\"\n    },\n    \"app_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Web URL for the project\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/bucketref-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: BucketRef
---
