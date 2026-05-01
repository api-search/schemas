---
description: ListNotificationsInput schema from AWS Well-Architected Tool API
layout: schema
name: ListNotificationsInput
properties_list:
- description: ''
  name: WorkloadId
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-list-notifications-input-schema.json
slug: well-architected-tool-list-notifications-input
source_filename: well-architected-tool-list-notifications-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"ListNotificationsInput\",\n  \"properties\": {\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListNotificationsMaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of results to return for this request.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-notifications-input-schema.json\",\n  \"description\": \"ListNotificationsInput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-notifications-input-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ListNotificationsInput
---
