---
description: A share invitation summary return object.
layout: schema
name: ShareInvitationSummary
properties_list:
- description: ''
  name: ShareInvitationId
  type: object
- description: ''
  name: SharedBy
  type: object
- description: ''
  name: SharedWith
  type: object
- description: ''
  name: PermissionType
  type: object
- description: ''
  name: ShareResourceType
  type: object
- description: ''
  name: WorkloadName
  type: object
- description: ''
  name: WorkloadId
  type: object
- description: ''
  name: LensName
  type: object
- description: ''
  name: LensArn
  type: object
- description: ''
  name: ProfileName
  type: object
- description: ''
  name: ProfileArn
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-share-invitation-summary-schema.json
slug: well-architected-tool-share-invitation-summary
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ShareInvitationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareInvitationId\"\n        },\n        {\n          \"description\": \"The ID assigned to the share invitation.\"\n        }\n      ]\n    },\n    \"SharedBy\": {\n      \"$ref\": \"#/components/schemas/AwsAccountId\"\n    },\n    \"SharedWith\": {\n      \"$ref\": \"#/components/schemas/SharedWith\"\n    },\n    \"PermissionType\": {\n      \"$ref\": \"#/components/schemas/PermissionType\"\n    },\n    \"ShareResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareResourceType\"\n        },\n        {\n          \"description\": \"The resource type of the share invitation.\"\n        }\n      ]\n    },\n    \"WorkloadName\": {\n      \"$ref\": \"#/components/schemas/WorkloadName\"\n    },\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    },\n    \"\
  LensName\": {\n      \"$ref\": \"#/components/schemas/LensName\"\n    },\n    \"LensArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"The ARN for the lens.\"\n        }\n      ]\n    },\n    \"ProfileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileName\"\n        },\n        {\n          \"description\": \"The profile name.\"\n        }\n      ]\n    },\n    \"ProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileArn\"\n        },\n        {\n          \"description\": \"The profile ARN.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A share invitation summary return object.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ShareInvitationSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-share-invitation-summary-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-share-invitation-summary-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ShareInvitationSummary
---
