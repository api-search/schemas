---
description: The profile choice.
layout: schema
name: ProfileChoice
properties_list:
- description: ''
  name: ChoiceId
  type: object
- description: ''
  name: ChoiceTitle
  type: object
- description: ''
  name: ChoiceDescription
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-profile-choice-schema.json
slug: well-architected-tool-profile-choice
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChoiceId\": {\n      \"$ref\": \"#/components/schemas/ChoiceId\"\n    },\n    \"ChoiceTitle\": {\n      \"$ref\": \"#/components/schemas/ChoiceTitle\"\n    },\n    \"ChoiceDescription\": {\n      \"$ref\": \"#/components/schemas/ChoiceDescription\"\n    }\n  },\n  \"description\": \"The profile choice.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProfileChoice\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-choice-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-choice-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ProfileChoice
---
