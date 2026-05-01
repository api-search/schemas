---
description: The profile notification summary.
layout: schema
name: ProfileNotificationSummary
properties_list:
- description: ''
  name: CurrentProfileVersion
  type: object
- description: ''
  name: LatestProfileVersion
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: ProfileArn
  type: object
- description: ''
  name: ProfileName
  type: object
- description: ''
  name: WorkloadId
  type: object
- description: ''
  name: WorkloadName
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-profile-notification-summary-schema.json
slug: well-architected-tool-profile-notification-summary
source_filename: well-architected-tool-profile-notification-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"CurrentProfileVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileVersion\"\n        },\n        {\n          \"description\": \"The current profile version.\"\n        }\n      ]\n    },\n    \"LatestProfileVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileVersion\"\n        },\n        {\n          \"description\": \"The latest profile version.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileNotificationType\"\n        },\n        {\n          \"description\": \"Type of notification.\"\n        }\n      ]\n    },\n    \"ProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileArn\"\n        },\n        {\n          \"description\": \"The profile ARN.\"\n        }\n      ]\n    },\n    \"ProfileName\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileName\"\n        },\n        {\n          \"description\": \"The profile name.\"\n        }\n      ]\n    },\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    },\n    \"WorkloadName\": {\n      \"$ref\": \"#/components/schemas/WorkloadName\"\n    }\n  },\n  \"description\": \"The profile notification summary.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProfileNotificationSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-notification-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-profile-notification-summary-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ProfileNotificationSummary
---
