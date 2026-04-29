---
description: An answer of the question.
layout: schema
name: Answer
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
  name: QuestionDescription
  type: object
- description: ''
  name: ImprovementPlanUrl
  type: object
- description: ''
  name: HelpfulResourceUrl
  type: object
- description: ''
  name: HelpfulResourceDisplayText
  type: object
- description: ''
  name: Choices
  type: object
- description: ''
  name: SelectedChoices
  type: object
- description: ''
  name: ChoiceAnswers
  type: object
- description: ''
  name: IsApplicable
  type: object
- description: ''
  name: Risk
  type: object
- description: ''
  name: Notes
  type: object
- description: ''
  name: Reason
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-answer-schema.json
slug: well-architected-tool-answer
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"QuestionId\": {\n      \"$ref\": \"#/components/schemas/QuestionId\"\n    },\n    \"PillarId\": {\n      \"$ref\": \"#/components/schemas/PillarId\"\n    },\n    \"QuestionTitle\": {\n      \"$ref\": \"#/components/schemas/QuestionTitle\"\n    },\n    \"QuestionDescription\": {\n      \"$ref\": \"#/components/schemas/QuestionDescription\"\n    },\n    \"ImprovementPlanUrl\": {\n      \"$ref\": \"#/components/schemas/ImprovementPlanUrl\"\n    },\n    \"HelpfulResourceUrl\": {\n      \"$ref\": \"#/components/schemas/HelpfulResourceUrl\"\n    },\n    \"HelpfulResourceDisplayText\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisplayText\"\n        },\n        {\n          \"description\": \"<p>The helpful resource text to be displayed for a custom lens.</p> <p>This field does not apply to Amazon Web Services official lenses.</p>\"\n        }\n      ]\n    },\n    \"Choices\": {\n      \"$ref\"\
  : \"#/components/schemas/Choices\"\n    },\n    \"SelectedChoices\": {\n      \"$ref\": \"#/components/schemas/SelectedChoices\"\n    },\n    \"ChoiceAnswers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceAnswers\"\n        },\n        {\n          \"description\": \"A list of selected choices to a question in your workload.\"\n        }\n      ]\n    },\n    \"IsApplicable\": {\n      \"$ref\": \"#/components/schemas/IsApplicable\"\n    },\n    \"Risk\": {\n      \"$ref\": \"#/components/schemas/Risk\"\n    },\n    \"Notes\": {\n      \"$ref\": \"#/components/schemas/Notes\"\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnswerReason\"\n        },\n        {\n          \"description\": \"The reason why the question is not applicable to your workload.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An answer of the question.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"Answer\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-answer-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-answer-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: Answer
---
