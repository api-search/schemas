---
description: A milestone return object.
layout: schema
name: Milestone
properties_list:
- description: ''
  name: MilestoneNumber
  type: object
- description: ''
  name: MilestoneName
  type: object
- description: ''
  name: RecordedAt
  type: object
- description: ''
  name: Workload
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-milestone-schema.json
slug: well-architected-tool-milestone
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"MilestoneNumber\": {\n      \"$ref\": \"#/components/schemas/MilestoneNumber\"\n    },\n    \"MilestoneName\": {\n      \"$ref\": \"#/components/schemas/MilestoneName\"\n    },\n    \"RecordedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"Workload\": {\n      \"$ref\": \"#/components/schemas/Workload\"\n    }\n  },\n  \"description\": \"A milestone return object.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Milestone\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-milestone-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-milestone-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: Milestone
---
