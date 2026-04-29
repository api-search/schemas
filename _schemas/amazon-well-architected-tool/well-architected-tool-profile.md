---
description: A profile.
layout: schema
name: Profile
properties_list:
- description: ''
  name: ProfileArn
  type: object
- description: ''
  name: ProfileVersion
  type: object
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
  name: Owner
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: UpdatedAt
  type: object
- description: ''
  name: ShareInvitationId
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-profile-schema.json
slug: well-architected-tool-profile
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileArn\"\n        },\n        {\n          \"description\": \"The profile ARN.\"\n        }\n      ]\n    },\n    \"ProfileVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileVersion\"\n        },\n        {\n          \"description\": \"The profile version.\"\n        }\n      ]\n    },\n    \"ProfileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileName\"\n        },\n        {\n          \"description\": \"The profile name.\"\n        }\n      ]\n    },\n    \"ProfileDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileDescription\"\n        },\n        {\n          \"description\": \"The profile description.\"\n        }\n      ]\n    },\n    \"ProfileQuestions\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/ProfileQuestions\"\n        },\n        {\n          \"description\": \"Profile questions.\"\n        }\n      ]\n    },\n    \"Owner\": {\n      \"$ref\": \"#/components/schemas/AwsAccountId\"\n    },\n    \"CreatedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"UpdatedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"ShareInvitationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareInvitationId\"\n        },\n        {\n          \"description\": \"The ID assigned to the share invitation.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags assigned to the profile.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A profile.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\"\
  : \"Profile\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: Profile
---
