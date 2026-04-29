---
description: A lens review summary of a workload.
layout: schema
name: LensReviewSummary
properties_list:
- description: ''
  name: LensAlias
  type: object
- description: ''
  name: LensArn
  type: object
- description: ''
  name: LensVersion
  type: object
- description: ''
  name: LensName
  type: object
- description: ''
  name: LensStatus
  type: object
- description: ''
  name: UpdatedAt
  type: object
- description: ''
  name: RiskCounts
  type: object
- description: ''
  name: Profiles
  type: object
- description: ''
  name: PrioritizedRiskCounts
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-lens-review-summary-schema.json
slug: well-architected-tool-lens-review-summary
source_filename: well-architected-tool-lens-review-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LensAlias\": {\n      \"$ref\": \"#/components/schemas/LensAlias\"\n    },\n    \"LensArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"The ARN for the lens.\"\n        }\n      ]\n    },\n    \"LensVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensVersion\"\n        },\n        {\n          \"description\": \"The version of the lens.\"\n        }\n      ]\n    },\n    \"LensName\": {\n      \"$ref\": \"#/components/schemas/LensName\"\n    },\n    \"LensStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensStatus\"\n        },\n        {\n          \"description\": \"The status of the lens.\"\n        }\n      ]\n    },\n    \"UpdatedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"RiskCounts\": {\n      \"$ref\": \"#/components/schemas/RiskCounts\"\
  \n    },\n    \"Profiles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkloadProfiles\"\n        },\n        {\n          \"description\": \"The profiles associated with the workload.\"\n        }\n      ]\n    },\n    \"PrioritizedRiskCounts\": {\n      \"$ref\": \"#/components/schemas/RiskCounts\"\n    }\n  },\n  \"description\": \"A lens review summary of a workload.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LensReviewSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-lens-review-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-lens-review-summary-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: LensReviewSummary
---
