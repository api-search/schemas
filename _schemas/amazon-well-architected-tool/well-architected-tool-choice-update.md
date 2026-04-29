---
description: A list of choices to be updated.
layout: schema
name: ChoiceUpdate
properties_list:
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
schema_file: json-schema/well-architected-tool-choice-update-schema.json
slug: well-architected-tool-choice-update
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"Status\"\n  ],\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceStatus\"\n        },\n        {\n          \"description\": \"The status of a choice.\"\n        }\n      ]\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceReason\"\n        },\n        {\n          \"description\": \"The reason why a choice is non-applicable to a question in your workload.\"\n        }\n      ]\n    },\n    \"Notes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceNotes\"\n        },\n        {\n          \"description\": \"The notes associated with a choice.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A list of choices to be updated.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChoiceUpdate\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-choice-update-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-choice-update-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ChoiceUpdate
---
