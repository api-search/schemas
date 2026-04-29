---
description: A profile question.
layout: schema
name: ProfileQuestion
properties_list:
- description: ''
  name: QuestionId
  type: object
- description: ''
  name: QuestionTitle
  type: object
- description: ''
  name: QuestionDescription
  type: object
- description: ''
  name: QuestionChoices
  type: object
- description: ''
  name: SelectedChoiceIds
  type: object
- description: ''
  name: MinSelectedChoices
  type: object
- description: ''
  name: MaxSelectedChoices
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-profile-question-schema.json
slug: well-architected-tool-profile-question
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"QuestionId\": {\n      \"$ref\": \"#/components/schemas/QuestionId\"\n    },\n    \"QuestionTitle\": {\n      \"$ref\": \"#/components/schemas/QuestionTitle\"\n    },\n    \"QuestionDescription\": {\n      \"$ref\": \"#/components/schemas/QuestionDescription\"\n    },\n    \"QuestionChoices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileQuestionChoices\"\n        },\n        {\n          \"description\": \"The question choices.\"\n        }\n      ]\n    },\n    \"SelectedChoiceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SelectedChoiceIds\"\n        },\n        {\n          \"description\": \"The selected choices.\"\n        }\n      ]\n    },\n    \"MinSelectedChoices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinSelectedProfileChoices\"\n        },\n        {\n          \"description\": \"The minimum number\
  \ of selected choices.\"\n        }\n      ]\n    },\n    \"MaxSelectedChoices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxSelectedProfileChoices\"\n        },\n        {\n          \"description\": \"The maximum number of selected choices.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A profile question.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProfileQuestion\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-question-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-question-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ProfileQuestion
---
