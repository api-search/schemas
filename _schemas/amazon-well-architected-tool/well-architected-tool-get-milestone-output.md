---
description: Output of a get milestone call.
layout: schema
name: GetMilestoneOutput
properties_list:
- description: ''
  name: WorkloadId
  type: object
- description: ''
  name: Milestone
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-get-milestone-output-schema.json
slug: well-architected-tool-get-milestone-output
source_filename: well-architected-tool-get-milestone-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    },\n    \"Milestone\": {\n      \"$ref\": \"#/components/schemas/Milestone\"\n    }\n  },\n  \"description\": \"Output of a get milestone call.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetMilestoneOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-milestone-output-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-milestone-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: GetMilestoneOutput
---
