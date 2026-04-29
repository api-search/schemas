---
description: A report of a lens review.
layout: schema
name: LensReviewReport
properties_list:
- description: ''
  name: LensAlias
  type: object
- description: ''
  name: LensArn
  type: object
- description: ''
  name: Base64String
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-lens-review-report-schema.json
slug: well-architected-tool-lens-review-report
source_filename: well-architected-tool-lens-review-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LensAlias\": {\n      \"$ref\": \"#/components/schemas/LensAlias\"\n    },\n    \"LensArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"The ARN for the lens.\"\n        }\n      ]\n    },\n    \"Base64String\": {\n      \"$ref\": \"#/components/schemas/Base64String\"\n    }\n  },\n  \"description\": \"A report of a lens review.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LensReviewReport\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-lens-review-report-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-lens-review-report-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: LensReviewReport
---
