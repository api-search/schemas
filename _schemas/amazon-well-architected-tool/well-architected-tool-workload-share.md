---
description: A workload share return object.
layout: schema
name: WorkloadShare
properties_list:
- description: ''
  name: ShareId
  type: object
- description: ''
  name: SharedBy
  type: object
- description: ''
  name: SharedWith
  type: object
- description: ''
  name: PermissionType
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: WorkloadName
  type: object
- description: ''
  name: WorkloadId
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-workload-share-schema.json
slug: well-architected-tool-workload-share
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ShareId\": {\n      \"$ref\": \"#/components/schemas/ShareId\"\n    },\n    \"SharedBy\": {\n      \"$ref\": \"#/components/schemas/AwsAccountId\"\n    },\n    \"SharedWith\": {\n      \"$ref\": \"#/components/schemas/SharedWith\"\n    },\n    \"PermissionType\": {\n      \"$ref\": \"#/components/schemas/PermissionType\"\n    },\n    \"Status\": {\n      \"$ref\": \"#/components/schemas/ShareStatus\"\n    },\n    \"WorkloadName\": {\n      \"$ref\": \"#/components/schemas/WorkloadName\"\n    },\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    }\n  },\n  \"description\": \"A workload share return object.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkloadShare\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-share-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-share-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: WorkloadShare
---
