---
description: Input to list all workloads.
layout: schema
name: ListWorkloadsInput
properties_list:
- description: ''
  name: WorkloadNamePrefix
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-list-workloads-input-schema.json
slug: well-architected-tool-list-workloads-input
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"ListWorkloadsInput\",\n  \"properties\": {\n    \"WorkloadNamePrefix\": {\n      \"$ref\": \"#/components/schemas/WorkloadNamePrefix\"\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListWorkloadsMaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of results to return for this request.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Input to list all workloads.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-workloads-input-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-workloads-input-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ListWorkloadsInput
---
