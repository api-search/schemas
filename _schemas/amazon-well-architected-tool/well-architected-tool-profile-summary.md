---
description: Summary of a profile.
layout: schema
name: ProfileSummary
properties_list:
- description: ''
  name: ProfileArn
  type: object
- description: ''
  name: ProfileVersion
  type: object
- description: ''
  name: ProfileName
  type: object
- description: ''
  name: ProfileDescription
  type: object
- description: ''
  name: Owner
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: UpdatedAt
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-profile-summary-schema.json
slug: well-architected-tool-profile-summary
source_filename: well-architected-tool-profile-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileArn\"\n        },\n        {\n          \"description\": \"The profile ARN.\"\n        }\n      ]\n    },\n    \"ProfileVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileVersion\"\n        },\n        {\n          \"description\": \"The profile version.\"\n        }\n      ]\n    },\n    \"ProfileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileName\"\n        },\n        {\n          \"description\": \"The profile name.\"\n        }\n      ]\n    },\n    \"ProfileDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileDescription\"\n        },\n        {\n          \"description\": \"The profile description.\"\n        }\n      ]\n    },\n    \"Owner\": {\n      \"$ref\": \"#/components/schemas/AwsAccountId\"\
  \n    },\n    \"CreatedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"UpdatedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    }\n  },\n  \"description\": \"Summary of a profile.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProfileSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-summary-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ProfileSummary
---
