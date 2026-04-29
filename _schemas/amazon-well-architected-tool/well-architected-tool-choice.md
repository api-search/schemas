---
description: A choice available to answer question.
layout: schema
name: Choice
properties_list:
- description: ''
  name: ChoiceId
  type: object
- description: ''
  name: Title
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: HelpfulResource
  type: object
- description: ''
  name: ImprovementPlan
  type: object
- description: ''
  name: AdditionalResources
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-choice-schema.json
slug: well-architected-tool-choice
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChoiceId\": {\n      \"$ref\": \"#/components/schemas/ChoiceId\"\n    },\n    \"Title\": {\n      \"$ref\": \"#/components/schemas/ChoiceTitle\"\n    },\n    \"Description\": {\n      \"$ref\": \"#/components/schemas/ChoiceDescription\"\n    },\n    \"HelpfulResource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceContent\"\n        },\n        {\n          \"description\": \"<p>The helpful resource (both text and URL) for a particular choice.</p> <p>This field only applies to custom lenses. Each choice can have only one helpful resource.</p>\"\n        }\n      ]\n    },\n    \"ImprovementPlan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceContent\"\n        },\n        {\n          \"description\": \"<p>The improvement plan (both text and URL) for a particular choice.</p> <p>This field only applies to custom lenses. Each choice can have only\
  \ one improvement plan.</p>\"\n        }\n      ]\n    },\n    \"AdditionalResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdditionalResourcesList\"\n        },\n        {\n          \"description\": \"<p>The additional resources for a choice in a custom lens.</p> <p>A choice can have up to two additional resources: one of type <code>HELPFUL_RESOURCE</code>, one of type <code>IMPROVEMENT_PLAN</code>, or both.</p>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A choice available to answer question.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Choice\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-choice-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-choice-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: Choice
---
