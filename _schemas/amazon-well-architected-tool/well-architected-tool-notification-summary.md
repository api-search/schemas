---
description: A notification summary return object.
layout: schema
name: NotificationSummary
properties_list:
- description: ''
  name: Type
  type: object
- description: ''
  name: LensUpgradeSummary
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-notification-summary-schema.json
slug: well-architected-tool-notification-summary
source_filename: well-architected-tool-notification-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationType\"\n        },\n        {\n          \"description\": \"The type of notification.\"\n        }\n      ]\n    },\n    \"LensUpgradeSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensUpgradeSummary\"\n        },\n        {\n          \"description\": \"Summary of lens upgrade.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A notification summary return object.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotificationSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-notification-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-notification-summary-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: NotificationSummary
---
