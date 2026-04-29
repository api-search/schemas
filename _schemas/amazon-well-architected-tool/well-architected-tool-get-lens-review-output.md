---
description: Output of a get lens review call.
layout: schema
name: GetLensReviewOutput
properties_list:
- description: ''
  name: WorkloadId
  type: object
- description: ''
  name: MilestoneNumber
  type: object
- description: ''
  name: LensReview
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-get-lens-review-output-schema.json
slug: well-architected-tool-get-lens-review-output
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    },\n    \"MilestoneNumber\": {\n      \"$ref\": \"#/components/schemas/MilestoneNumber\"\n    },\n    \"LensReview\": {\n      \"$ref\": \"#/components/schemas/LensReview\"\n    }\n  },\n  \"description\": \"Output of a get lens review call.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetLensReviewOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-lens-review-output-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-lens-review-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: GetLensReviewOutput
---
