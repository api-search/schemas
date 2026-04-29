---
description: Request body for creating a new lifecycle policy.
layout: schema
name: Create Lifecycle Policy Request
properties_list:
- description: ''
  name: Description
  type: string
- description: ''
  name: State
  type: string
- description: ''
  name: ExecutionRoleArn
  type: string
- description: ''
  name: PolicyDetails
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Data Lifecycle Manager
provider_slug: amazon-data-lifecycle-manager
schema_file: json-schema/create-lifecycle-policy-request-schema.json
slug: create-lifecycle-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-lifecycle-manager/json-schema/create-lifecycle-policy-request-schema.json\",\n  \"title\": \"Create Lifecycle Policy Request\",\n  \"description\": \"Request body for creating a new lifecycle policy.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"Description\",\n    \"State\",\n    \"ExecutionRoleArn\",\n    \"PolicyDetails\"\n  ],\n  \"properties\": {\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\"\n      ]\n    },\n    \"ExecutionRoleArn\": {\n      \"type\": \"string\"\n    },\n    \"PolicyDetails\": {\n      \"type\": \"object\"\n    },\n    \"Tags\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-lifecycle-manager/refs/heads/main/json-schema/create-lifecycle-policy-request-schema.json
tags:
- AWS
- Backup
- EBS Snapshots
- Lifecycle Management
- Storage
- Automation
- Compliance
title: Create Lifecycle Policy Request
---
