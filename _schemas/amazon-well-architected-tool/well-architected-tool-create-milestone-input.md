---
description: Input for milestone creation.
layout: schema
name: CreateMilestoneInput
properties_list:
- description: ''
  name: MilestoneName
  type: object
- description: ''
  name: ClientRequestToken
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-create-milestone-input-schema.json
slug: well-architected-tool-create-milestone-input
source_filename: well-architected-tool-create-milestone-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"MilestoneName\",\n    \"ClientRequestToken\"\n  ],\n  \"title\": \"CreateMilestoneInput\",\n  \"properties\": {\n    \"MilestoneName\": {\n      \"$ref\": \"#/components/schemas/MilestoneName\"\n    },\n    \"ClientRequestToken\": {\n      \"$ref\": \"#/components/schemas/ClientRequestToken\"\n    }\n  },\n  \"description\": \"Input for milestone creation.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-milestone-input-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-milestone-input-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: CreateMilestoneInput
---
