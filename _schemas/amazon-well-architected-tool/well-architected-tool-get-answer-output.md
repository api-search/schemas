---
description: Output of a get answer call.
layout: schema
name: GetAnswerOutput
properties_list:
- description: ''
  name: WorkloadId
  type: object
- description: ''
  name: MilestoneNumber
  type: object
- description: ''
  name: LensAlias
  type: object
- description: ''
  name: LensArn
  type: object
- description: ''
  name: Answer
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-get-answer-output-schema.json
slug: well-architected-tool-get-answer-output
source_filename: well-architected-tool-get-answer-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    },\n    \"MilestoneNumber\": {\n      \"$ref\": \"#/components/schemas/MilestoneNumber\"\n    },\n    \"LensAlias\": {\n      \"$ref\": \"#/components/schemas/LensAlias\"\n    },\n    \"LensArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"The ARN for the lens.\"\n        }\n      ]\n    },\n    \"Answer\": {\n      \"$ref\": \"#/components/schemas/Answer\"\n    }\n  },\n  \"description\": \"Output of a get answer call.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetAnswerOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-answer-output-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-answer-output-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: GetAnswerOutput
---
