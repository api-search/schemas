---
description: A pillar review summary of a lens review.
layout: schema
name: PillarReviewSummary
properties_list:
- description: ''
  name: PillarId
  type: object
- description: ''
  name: PillarName
  type: object
- description: ''
  name: Notes
  type: object
- description: ''
  name: RiskCounts
  type: object
- description: ''
  name: PrioritizedRiskCounts
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-pillar-review-summary-schema.json
slug: well-architected-tool-pillar-review-summary
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"PillarId\": {\n      \"$ref\": \"#/components/schemas/PillarId\"\n    },\n    \"PillarName\": {\n      \"$ref\": \"#/components/schemas/PillarName\"\n    },\n    \"Notes\": {\n      \"$ref\": \"#/components/schemas/Notes\"\n    },\n    \"RiskCounts\": {\n      \"$ref\": \"#/components/schemas/RiskCounts\"\n    },\n    \"PrioritizedRiskCounts\": {\n      \"$ref\": \"#/components/schemas/RiskCounts\"\n    }\n  },\n  \"description\": \"A pillar review summary of a lens review.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PillarReviewSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-pillar-review-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-pillar-review-summary-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: PillarReviewSummary
---
