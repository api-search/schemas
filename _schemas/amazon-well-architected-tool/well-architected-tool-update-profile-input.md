---
description: UpdateProfileInput schema from AWS Well-Architected Tool API
layout: schema
name: UpdateProfileInput
properties_list:
- description: ''
  name: ProfileDescription
  type: object
- description: ''
  name: ProfileQuestions
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-update-profile-input-schema.json
slug: well-architected-tool-update-profile-input
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"UpdateProfileInput\",\n  \"properties\": {\n    \"ProfileDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileDescription\"\n        },\n        {\n          \"description\": \"The profile description.\"\n        }\n      ]\n    },\n    \"ProfileQuestions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileQuestionUpdates\"\n        },\n        {\n          \"description\": \"Profile questions.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-update-profile-input-schema.json\",\n  \"description\": \"UpdateProfileInput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-update-profile-input-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: UpdateProfileInput
---
