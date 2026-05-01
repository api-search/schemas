---
description: A metric for a particular question in the pillar.
layout: schema
name: QuestionMetric
properties_list:
- description: ''
  name: QuestionId
  type: object
- description: ''
  name: Risk
  type: object
- description: ''
  name: BestPractices
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-question-metric-schema.json
slug: well-architected-tool-question-metric
source_filename: well-architected-tool-question-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"QuestionId\": {\n      \"$ref\": \"#/components/schemas/QuestionId\"\n    },\n    \"Risk\": {\n      \"$ref\": \"#/components/schemas/Risk\"\n    },\n    \"BestPractices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BestPractices\"\n        },\n        {\n          \"description\": \"The best practices, or choices, that have been identified as contributing to risk in a question.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A metric for a particular question in the pillar. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QuestionMetric\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-question-metric-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-question-metric-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: QuestionMetric
---
