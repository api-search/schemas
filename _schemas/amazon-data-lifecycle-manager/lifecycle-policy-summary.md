---
description: Summary information about a lifecycle policy.
layout: schema
name: Lifecycle Policy Summary
properties_list:
- description: The identifier of the lifecycle policy
  name: PolicyId
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: State
  type: string
- description: ''
  name: PolicyType
  type: string
- description: ''
  name: PolicySummary
  type: string
provider_name: Amazon Data Lifecycle Manager
provider_slug: amazon-data-lifecycle-manager
schema_file: json-schema/lifecycle-policy-summary-schema.json
slug: lifecycle-policy-summary
source_filename: lifecycle-policy-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-lifecycle-manager/json-schema/lifecycle-policy-summary-schema.json\",\n  \"title\": \"Lifecycle Policy Summary\",\n  \"description\": \"Summary information about a lifecycle policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the lifecycle policy\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\",\n        \"ERROR\"\n      ]\n    },\n    \"PolicyType\": {\n      \"type\": \"string\"\n    },\n    \"PolicySummary\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-lifecycle-manager/refs/heads/main/json-schema/lifecycle-policy-summary-schema.json
tags:
- AWS
- Backup
- EBS Snapshots
- Lifecycle Management
- Storage
- Automation
- Compliance
title: Lifecycle Policy Summary
---
