---
description: Request body for creating a compute fleet.
layout: schema
name: Create Fleet Request
properties_list:
- description: ''
  name: displayName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: roleArn
  type: string
- description: ''
  name: configuration
  type: object
- description: ''
  name: minWorkerCount
  type: integer
- description: ''
  name: maxWorkerCount
  type: integer
provider_name: Amazon Deadline Cloud
provider_slug: amazon-deadline-cloud
schema_file: json-schema/create-fleet-request-schema.json
slug: create-fleet-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deadline-cloud/json-schema/create-fleet-request-schema.json\",\n  \"title\": \"Create Fleet Request\",\n  \"description\": \"Request body for creating a compute fleet.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"displayName\",\n    \"roleArn\",\n    \"configuration\"\n  ],\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"roleArn\": {\n      \"type\": \"string\"\n    },\n    \"configuration\": {\n      \"type\": \"object\"\n    },\n    \"minWorkerCount\": {\n      \"type\": \"integer\"\n    },\n    \"maxWorkerCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/json-schema/create-fleet-request-schema.json
tags:
- AWS
- Compute
- Media
- Rendering
- Visual Effects
title: Create Fleet Request
---
