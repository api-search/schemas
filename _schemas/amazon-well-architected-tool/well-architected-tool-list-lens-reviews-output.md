---
description: Output of a list lens reviews call.
layout: schema
name: ListLensReviewsOutput
properties_list:
- description: ''
  name: WorkloadId
  type: object
- description: ''
  name: MilestoneNumber
  type: object
- description: ''
  name: LensReviewSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-list-lens-reviews-output-schema.json
slug: well-architected-tool-list-lens-reviews-output
source_filename: well-architected-tool-list-lens-reviews-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    },\n    \"MilestoneNumber\": {\n      \"$ref\": \"#/components/schemas/MilestoneNumber\"\n    },\n    \"LensReviewSummaries\": {\n      \"$ref\": \"#/components/schemas/LensReviewSummaries\"\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    }\n  },\n  \"description\": \"Output of a list lens reviews call.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListLensReviewsOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-lens-reviews-output-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-lens-reviews-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ListLensReviewsOutput
---
