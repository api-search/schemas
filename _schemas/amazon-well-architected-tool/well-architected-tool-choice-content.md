---
description: The choice content.
layout: schema
name: ChoiceContent
properties_list:
- description: ''
  name: DisplayText
  type: object
- description: ''
  name: Url
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-choice-content-schema.json
slug: well-architected-tool-choice-content
source_filename: well-architected-tool-choice-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DisplayText\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceContentDisplayText\"\n        },\n        {\n          \"description\": \"The display text for the choice content.\"\n        }\n      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChoiceContentUrl\"\n        },\n        {\n          \"description\": \"The URL for the choice content.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The choice content.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChoiceContent\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-choice-content-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-choice-content-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ChoiceContent
---
