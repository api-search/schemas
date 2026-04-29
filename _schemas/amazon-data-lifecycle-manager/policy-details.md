---
description: Specifies the configuration of a lifecycle policy.
layout: schema
name: Policy Details
properties_list:
- description: ''
  name: PolicyType
  type: string
- description: ''
  name: ResourceTypes
  type: array
- description: ''
  name: TargetTags
  type: array
- description: ''
  name: Schedules
  type: array
provider_name: Amazon Data Lifecycle Manager
provider_slug: amazon-data-lifecycle-manager
schema_file: json-schema/policy-details-schema.json
slug: policy-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-lifecycle-manager/json-schema/policy-details-schema.json\",\n  \"title\": \"Policy Details\",\n  \"description\": \"Specifies the configuration of a lifecycle policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"EBS_SNAPSHOT_MANAGEMENT\",\n        \"IMAGE_MANAGEMENT\",\n        \"EVENT_BASED_POLICY\"\n      ]\n    },\n    \"ResourceTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"TargetTags\": {\n      \"type\": \"array\"\n    },\n    \"Schedules\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-lifecycle-manager/refs/heads/main/json-schema/policy-details-schema.json
tags:
- AWS
- Backup
- EBS Snapshots
- Lifecycle Management
- Storage
- Automation
- Compliance
title: Policy Details
---
