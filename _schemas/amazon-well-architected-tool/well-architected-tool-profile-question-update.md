---
description: An update to a profile question.
layout: schema
name: ProfileQuestionUpdate
properties_list:
- description: ''
  name: QuestionId
  type: object
- description: ''
  name: SelectedChoiceIds
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-profile-question-update-schema.json
slug: well-architected-tool-profile-question-update
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"QuestionId\": {\n      \"$ref\": \"#/components/schemas/QuestionId\"\n    },\n    \"SelectedChoiceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SelectedProfileChoiceIds\"\n        },\n        {\n          \"description\": \"The selected choices.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An update to a profile question.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProfileQuestionUpdate\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-question-update-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-question-update-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ProfileQuestionUpdate
---
