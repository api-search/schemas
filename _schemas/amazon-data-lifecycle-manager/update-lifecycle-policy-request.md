---
description: Request body for updating a lifecycle policy.
layout: schema
name: Update Lifecycle Policy Request
properties_list:
- description: ''
  name: State
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: ExecutionRoleArn
  type: string
- description: ''
  name: PolicyDetails
  type: object
provider_name: Amazon Data Lifecycle Manager
provider_slug: amazon-data-lifecycle-manager
schema_file: json-schema/update-lifecycle-policy-request-schema.json
slug: update-lifecycle-policy-request
source_filename: update-lifecycle-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-lifecycle-manager/json-schema/update-lifecycle-policy-request-schema.json\",\n  \"title\": \"Update Lifecycle Policy Request\",\n  \"description\": \"Request body for updating a lifecycle policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"State\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\"\n      ]\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"ExecutionRoleArn\": {\n      \"type\": \"string\"\n    },\n    \"PolicyDetails\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-lifecycle-manager/refs/heads/main/json-schema/update-lifecycle-policy-request-schema.json
tags:
- AWS
- Backup
- EBS Snapshots
- Lifecycle Management
- Storage
- Automation
- Compliance
title: Update Lifecycle Policy Request
---
