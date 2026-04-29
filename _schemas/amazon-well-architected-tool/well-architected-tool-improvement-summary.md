---
description: An improvement summary of a lens review in a workload.
layout: schema
name: ImprovementSummary
properties_list:
- description: ''
  name: QuestionId
  type: object
- description: ''
  name: PillarId
  type: object
- description: ''
  name: QuestionTitle
  type: object
- description: ''
  name: Risk
  type: object
- description: ''
  name: ImprovementPlanUrl
  type: object
- description: ''
  name: ImprovementPlans
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-improvement-summary-schema.json
slug: well-architected-tool-improvement-summary
source_filename: well-architected-tool-improvement-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"QuestionId\": {\n      \"$ref\": \"#/components/schemas/QuestionId\"\n    },\n    \"PillarId\": {\n      \"$ref\": \"#/components/schemas/PillarId\"\n    },\n    \"QuestionTitle\": {\n      \"$ref\": \"#/components/schemas/QuestionTitle\"\n    },\n    \"Risk\": {\n      \"$ref\": \"#/components/schemas/Risk\"\n    },\n    \"ImprovementPlanUrl\": {\n      \"$ref\": \"#/components/schemas/ImprovementPlanUrl\"\n    },\n    \"ImprovementPlans\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceImprovementPlans\"\n        },\n        {\n          \"description\": \"The improvement plan details.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An improvement summary of a lens review in a workload.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImprovementSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-improvement-summary-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-improvement-summary-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ImprovementSummary
---
