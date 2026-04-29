---
description: Output of a list workloads call.
layout: schema
name: ListWorkloadsOutput
properties_list:
- description: ''
  name: WorkloadSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-list-workloads-output-schema.json
slug: well-architected-tool-list-workloads-output
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkloadSummaries\": {\n      \"$ref\": \"#/components/schemas/WorkloadSummaries\"\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    }\n  },\n  \"description\": \"Output of a list workloads call.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListWorkloadsOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-workloads-output-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-workloads-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ListWorkloadsOutput
---
