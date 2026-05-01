---
description: Input to list all milestones for a workload.
layout: schema
name: ListMilestonesInput
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-list-milestones-input-schema.json
slug: well-architected-tool-list-milestones-input
source_filename: well-architected-tool-list-milestones-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"ListMilestonesInput\",\n  \"properties\": {\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    },\n    \"MaxResults\": {\n      \"$ref\": \"#/components/schemas/MaxResults\"\n    }\n  },\n  \"description\": \"Input to list all milestones for a workload.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-milestones-input-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-milestones-input-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ListMilestonesInput
---
