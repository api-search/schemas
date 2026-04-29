---
description: CreateProfileInput schema from AWS Well-Architected Tool API
layout: schema
name: CreateProfileInput
properties_list:
- description: ''
  name: ProfileName
  type: object
- description: ''
  name: ProfileDescription
  type: object
- description: ''
  name: ProfileQuestions
  type: object
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-create-profile-input-schema.json
slug: well-architected-tool-create-profile-input
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ProfileName\",\n    \"ProfileDescription\",\n    \"ProfileQuestions\",\n    \"ClientRequestToken\"\n  ],\n  \"title\": \"CreateProfileInput\",\n  \"properties\": {\n    \"ProfileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileName\"\n        },\n        {\n          \"description\": \"Name of the profile.\"\n        }\n      ]\n    },\n    \"ProfileDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileDescription\"\n        },\n        {\n          \"description\": \"The profile description.\"\n        }\n      ]\n    },\n    \"ProfileQuestions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileQuestionUpdates\"\n        },\n        {\n          \"description\": \"The profile questions.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"$ref\": \"#/components/schemas/ClientRequestToken\"\
  \n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags assigned to the profile.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-profile-input-schema.json\",\n  \"description\": \"CreateProfileInput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-profile-input-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: CreateProfileInput
---
