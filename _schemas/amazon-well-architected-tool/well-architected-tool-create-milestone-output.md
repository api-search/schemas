---
description: Output of a create milestone call.
layout: schema
name: CreateMilestoneOutput
properties_list:
- description: ''
  name: WorkloadId
  type: object
- description: ''
  name: MilestoneNumber
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-create-milestone-output-schema.json
slug: well-architected-tool-create-milestone-output
source_filename: well-architected-tool-create-milestone-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    },\n    \"MilestoneNumber\": {\n      \"$ref\": \"#/components/schemas/MilestoneNumber\"\n    }\n  },\n  \"description\": \"Output of a create milestone call.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateMilestoneOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-milestone-output-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-milestone-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: CreateMilestoneOutput
---
