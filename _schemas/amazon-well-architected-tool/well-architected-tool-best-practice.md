---
description: A best practice, or question choice, that has been identified as a risk in this question.
layout: schema
name: BestPractice
properties_list:
- description: ''
  name: ChoiceId
  type: object
- description: ''
  name: ChoiceTitle
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-best-practice-schema.json
slug: well-architected-tool-best-practice
source_filename: well-architected-tool-best-practice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChoiceId\": {\n      \"$ref\": \"#/components/schemas/ChoiceId\"\n    },\n    \"ChoiceTitle\": {\n      \"$ref\": \"#/components/schemas/ChoiceTitle\"\n    }\n  },\n  \"description\": \"A best practice, or question choice, that has been identified as a risk in this question.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BestPractice\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-best-practice-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-best-practice-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: BestPractice
---
