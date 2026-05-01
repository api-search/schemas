---
description: ListNotificationsOutput schema from AWS Well-Architected Tool API
layout: schema
name: ListNotificationsOutput
properties_list:
- description: ''
  name: NotificationSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-list-notifications-output-schema.json
slug: well-architected-tool-list-notifications-output
source_filename: well-architected-tool-list-notifications-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"NotificationSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationSummaries\"\n        },\n        {\n          \"description\": \"List of lens notification summaries in a workload.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListNotificationsOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-notifications-output-schema.json\",\n  \"description\": \"ListNotificationsOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-notifications-output-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ListNotificationsOutput
---
