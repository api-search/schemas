---
description: An answer summary of a lens review in a workload.
layout: schema
name: AnswerSummary
properties_list:
- description: ''
  name: QuestionId
  type: object
- description: ''
  name: PillarId
  type: object
- description: ''
  name: QuestionTitle
  type: object
- description: ''
  name: Choices
  type: object
- description: ''
  name: SelectedChoices
  type: object
- description: ''
  name: ChoiceAnswerSummaries
  type: object
- description: ''
  name: IsApplicable
  type: object
- description: ''
  name: Risk
  type: object
- description: ''
  name: Reason
  type: object
- description: ''
  name: QuestionType
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-answer-summary-schema.json
slug: well-architected-tool-answer-summary
source_filename: well-architected-tool-answer-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"QuestionId\": {\n      \"$ref\": \"#/components/schemas/QuestionId\"\n    },\n    \"PillarId\": {\n      \"$ref\": \"#/components/schemas/PillarId\"\n    },\n    \"QuestionTitle\": {\n      \"$ref\": \"#/components/schemas/QuestionTitle\"\n    },\n    \"Choices\": {\n      \"$ref\": \"#/components/schemas/Choices\"\n    },\n    \"SelectedChoices\": {\n      \"$ref\": \"#/components/schemas/SelectedChoices\"\n    },\n    \"ChoiceAnswerSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceAnswerSummaries\"\n        },\n        {\n          \"description\": \"A list of selected choices to a question in your workload.\"\n        }\n      ]\n    },\n    \"IsApplicable\": {\n      \"$ref\": \"#/components/schemas/IsApplicable\"\n    },\n    \"Risk\": {\n      \"$ref\": \"#/components/schemas/Risk\"\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnswerReason\"\
  \n        },\n        {\n          \"description\": \"The reason why a choice is non-applicable to a question in your workload.\"\n        }\n      ]\n    },\n    \"QuestionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QuestionType\"\n        },\n        {\n          \"description\": \"The type of the question.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An answer summary of a lens review in a workload.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AnswerSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-answer-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-answer-summary-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: AnswerSummary
---
