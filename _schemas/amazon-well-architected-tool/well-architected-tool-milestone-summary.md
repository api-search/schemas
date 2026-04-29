---
description: A milestone summary return object.
layout: schema
name: MilestoneSummary
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
  name: WorkloadSummary
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-milestone-summary-schema.json
slug: well-architected-tool-milestone-summary
source_filename: well-architected-tool-milestone-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"MilestoneNumber\": {\n      \"$ref\": \"#/components/schemas/MilestoneNumber\"\n    },\n    \"MilestoneName\": {\n      \"$ref\": \"#/components/schemas/MilestoneName\"\n    },\n    \"RecordedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"WorkloadSummary\": {\n      \"$ref\": \"#/components/schemas/WorkloadSummary\"\n    }\n  },\n  \"description\": \"A milestone summary return object.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MilestoneSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-milestone-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-milestone-summary-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: MilestoneSummary
---
