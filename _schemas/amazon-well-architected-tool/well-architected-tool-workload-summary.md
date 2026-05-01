---
description: A workload summary return object.
layout: schema
name: WorkloadSummary
properties_list:
- description: ''
  name: WorkloadId
  type: object
- description: ''
  name: WorkloadArn
  type: object
- description: ''
  name: WorkloadName
  type: object
- description: ''
  name: Owner
  type: object
- description: ''
  name: UpdatedAt
  type: object
- description: ''
  name: Lenses
  type: object
- description: ''
  name: RiskCounts
  type: object
- description: ''
  name: ImprovementStatus
  type: object
- description: ''
  name: Profiles
  type: object
- description: ''
  name: PrioritizedRiskCounts
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-workload-summary-schema.json
slug: well-architected-tool-workload-summary
source_filename: well-architected-tool-workload-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    },\n    \"WorkloadArn\": {\n      \"$ref\": \"#/components/schemas/WorkloadArn\"\n    },\n    \"WorkloadName\": {\n      \"$ref\": \"#/components/schemas/WorkloadName\"\n    },\n    \"Owner\": {\n      \"$ref\": \"#/components/schemas/AwsAccountId\"\n    },\n    \"UpdatedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"Lenses\": {\n      \"$ref\": \"#/components/schemas/WorkloadLenses\"\n    },\n    \"RiskCounts\": {\n      \"$ref\": \"#/components/schemas/RiskCounts\"\n    },\n    \"ImprovementStatus\": {\n      \"$ref\": \"#/components/schemas/WorkloadImprovementStatus\"\n    },\n    \"Profiles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkloadProfiles\"\n        },\n        {\n          \"description\": \"Profile associated with a workload.\"\n        }\n      ]\n    },\n    \"PrioritizedRiskCounts\"\
  : {\n      \"$ref\": \"#/components/schemas/RiskCounts\"\n    }\n  },\n  \"description\": \"A workload summary return object.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkloadSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-summary-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: WorkloadSummary
---
