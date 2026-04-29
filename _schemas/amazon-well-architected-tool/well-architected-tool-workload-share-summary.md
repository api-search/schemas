---
description: A workload share summary return object.
layout: schema
name: WorkloadShareSummary
properties_list:
- description: ''
  name: ShareId
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
  name: StatusMessage
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-workload-share-summary-schema.json
slug: well-architected-tool-workload-share-summary
source_filename: well-architected-tool-workload-share-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ShareId\": {\n      \"$ref\": \"#/components/schemas/ShareId\"\n    },\n    \"SharedWith\": {\n      \"$ref\": \"#/components/schemas/SharedWith\"\n    },\n    \"PermissionType\": {\n      \"$ref\": \"#/components/schemas/PermissionType\"\n    },\n    \"Status\": {\n      \"$ref\": \"#/components/schemas/ShareStatus\"\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusMessage\"\n        },\n        {\n          \"description\": \"Optional message to compliment the Status field.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A workload share summary return object.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkloadShareSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-share-summary-schema.json\"\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-share-summary-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: WorkloadShareSummary
---
