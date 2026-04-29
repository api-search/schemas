---
description: A metric for a particular lens in a workload.
layout: schema
name: LensMetric
properties_list:
- description: ''
  name: LensArn
  type: object
- description: ''
  name: Pillars
  type: object
- description: ''
  name: RiskCounts
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-lens-metric-schema.json
slug: well-architected-tool-lens-metric
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LensArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"The lens ARN.\"\n        }\n      ]\n    },\n    \"Pillars\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PillarMetrics\"\n        },\n        {\n          \"description\": \"The metrics for the pillars in a lens.\"\n        }\n      ]\n    },\n    \"RiskCounts\": {\n      \"$ref\": \"#/components/schemas/RiskCounts\"\n    }\n  },\n  \"description\": \"A metric for a particular lens in a workload.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LensMetric\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-lens-metric-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-lens-metric-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: LensMetric
---
