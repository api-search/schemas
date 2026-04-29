---
description: Input for update lens review.
layout: schema
name: UpdateLensReviewInput
properties_list:
- description: ''
  name: LensNotes
  type: object
- description: ''
  name: PillarNotes
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-update-lens-review-input-schema.json
slug: well-architected-tool-update-lens-review-input
source_filename: well-architected-tool-update-lens-review-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"UpdateLensReviewInput\",\n  \"properties\": {\n    \"LensNotes\": {\n      \"$ref\": \"#/components/schemas/Notes\"\n    },\n    \"PillarNotes\": {\n      \"$ref\": \"#/components/schemas/PillarNotes\"\n    }\n  },\n  \"description\": \"Input for update lens review.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-update-lens-review-input-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-update-lens-review-input-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: UpdateLensReviewInput
---
