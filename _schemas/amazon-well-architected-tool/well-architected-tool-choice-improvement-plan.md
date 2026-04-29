---
description: The choice level improvement plan.
layout: schema
name: ChoiceImprovementPlan
properties_list:
- description: ''
  name: ChoiceId
  type: object
- description: ''
  name: DisplayText
  type: object
- description: ''
  name: ImprovementPlanUrl
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-choice-improvement-plan-schema.json
slug: well-architected-tool-choice-improvement-plan
source_filename: well-architected-tool-choice-improvement-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChoiceId\": {\n      \"$ref\": \"#/components/schemas/ChoiceId\"\n    },\n    \"DisplayText\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisplayText\"\n        },\n        {\n          \"description\": \"The display text for the improvement plan.\"\n        }\n      ]\n    },\n    \"ImprovementPlanUrl\": {\n      \"$ref\": \"#/components/schemas/ImprovementPlanUrl\"\n    }\n  },\n  \"description\": \"The choice level improvement plan.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChoiceImprovementPlan\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-choice-improvement-plan-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-choice-improvement-plan-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ChoiceImprovementPlan
---
