---
description: The profile template.
layout: schema
name: ProfileTemplate
properties_list:
- description: ''
  name: TemplateName
  type: object
- description: ''
  name: TemplateQuestions
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: UpdatedAt
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-profile-template-schema.json
slug: well-architected-tool-profile-template
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"TemplateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileName\"\n        },\n        {\n          \"description\": \"The name of the profile template.\"\n        }\n      ]\n    },\n    \"TemplateQuestions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateQuestions\"\n        },\n        {\n          \"description\": \"Profile template questions.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"UpdatedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    }\n  },\n  \"description\": \"The profile template.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProfileTemplate\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-template-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-template-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ProfileTemplate
---
