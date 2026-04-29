---
description: A choice that has been answered on a question in your workload.
layout: schema
name: ChoiceAnswer
properties_list:
- description: ''
  name: ChoiceId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Reason
  type: object
- description: ''
  name: Notes
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-choice-answer-schema.json
slug: well-architected-tool-choice-answer
source_filename: well-architected-tool-choice-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChoiceId\": {\n      \"$ref\": \"#/components/schemas/ChoiceId\"\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceStatus\"\n        },\n        {\n          \"description\": \"The status of a choice.\"\n        }\n      ]\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceReason\"\n        },\n        {\n          \"description\": \"The reason why a choice is non-applicable to a question in your workload.\"\n        }\n      ]\n    },\n    \"Notes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceNotes\"\n        },\n        {\n          \"description\": \"The notes associated with a choice.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A choice that has been answered on a question in your workload.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"ChoiceAnswer\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-choice-answer-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-choice-answer-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ChoiceAnswer
---
