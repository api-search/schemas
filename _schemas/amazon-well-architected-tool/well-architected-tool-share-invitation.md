---
description: The share invitation.
layout: schema
name: ShareInvitation
properties_list:
- description: ''
  name: ShareInvitationId
  type: object
- description: ''
  name: ShareResourceType
  type: object
- description: ''
  name: WorkloadId
  type: object
- description: ''
  name: LensAlias
  type: object
- description: ''
  name: LensArn
  type: object
- description: ''
  name: ProfileArn
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-share-invitation-schema.json
slug: well-architected-tool-share-invitation
source_filename: well-architected-tool-share-invitation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ShareInvitationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareInvitationId\"\n        },\n        {\n          \"description\": \"The ID assigned to the share invitation.\"\n        }\n      ]\n    },\n    \"ShareResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareResourceType\"\n        },\n        {\n          \"description\": \"The resource type of the share invitation.\"\n        }\n      ]\n    },\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    },\n    \"LensAlias\": {\n      \"$ref\": \"#/components/schemas/LensAlias\"\n    },\n    \"LensArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"The ARN for the lens.\"\n        }\n      ]\n    },\n    \"ProfileArn\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/ProfileArn\"\n        },\n        {\n          \"description\": \"The profile ARN.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The share invitation.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ShareInvitation\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-share-invitation-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-share-invitation-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ShareInvitation
---
