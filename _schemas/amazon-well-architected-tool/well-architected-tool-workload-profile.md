---
description: The profile associated with a workload.
layout: schema
name: WorkloadProfile
properties_list:
- description: ''
  name: ProfileArn
  type: object
- description: ''
  name: ProfileVersion
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-workload-profile-schema.json
slug: well-architected-tool-workload-profile
source_filename: well-architected-tool-workload-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileArn\"\n        },\n        {\n          \"description\": \"The profile ARN.\"\n        }\n      ]\n    },\n    \"ProfileVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileVersion\"\n        },\n        {\n          \"description\": \"The profile version.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The profile associated with a workload.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkloadProfile\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-profile-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-profile-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: WorkloadProfile
---
