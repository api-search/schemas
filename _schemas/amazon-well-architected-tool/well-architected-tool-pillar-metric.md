---
description: A metric for a particular pillar in a lens.
layout: schema
name: PillarMetric
properties_list:
- description: ''
  name: PillarId
  type: object
- description: ''
  name: RiskCounts
  type: object
- description: ''
  name: Questions
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-pillar-metric-schema.json
slug: well-architected-tool-pillar-metric
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"PillarId\": {\n      \"$ref\": \"#/components/schemas/PillarId\"\n    },\n    \"RiskCounts\": {\n      \"$ref\": \"#/components/schemas/RiskCounts\"\n    },\n    \"Questions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QuestionMetrics\"\n        },\n        {\n          \"description\": \"The questions that have been identified as risks in the pillar.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A metric for a particular pillar in a lens.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PillarMetric\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-pillar-metric-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-pillar-metric-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: PillarMetric
---
