---
description: Input to update answer.
layout: schema
name: UpdateAnswerInput
properties_list:
- description: ''
  name: SelectedChoices
  type: object
- description: ''
  name: ChoiceUpdates
  type: object
- description: ''
  name: Notes
  type: object
- description: ''
  name: IsApplicable
  type: object
- description: ''
  name: Reason
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-update-answer-input-schema.json
slug: well-architected-tool-update-answer-input
source_filename: well-architected-tool-update-answer-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"UpdateAnswerInput\",\n  \"properties\": {\n    \"SelectedChoices\": {\n      \"$ref\": \"#/components/schemas/SelectedChoices\"\n    },\n    \"ChoiceUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceUpdates\"\n        },\n        {\n          \"description\": \"A list of choices to update on a question in your workload. The String key corresponds to the choice ID to be updated.\"\n        }\n      ]\n    },\n    \"Notes\": {\n      \"$ref\": \"#/components/schemas/Notes\"\n    },\n    \"IsApplicable\": {\n      \"$ref\": \"#/components/schemas/IsApplicable\"\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnswerReason\"\n        },\n        {\n          \"description\": \"The reason why a question is not applicable to your workload.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Input to update answer.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-update-answer-input-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-update-answer-input-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: UpdateAnswerInput
---
