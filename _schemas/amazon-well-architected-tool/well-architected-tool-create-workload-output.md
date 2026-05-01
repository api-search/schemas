---
description: Output of a create workload call.
layout: schema
name: CreateWorkloadOutput
properties_list:
- description: ''
  name: WorkloadId
  type: object
- description: ''
  name: WorkloadArn
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-create-workload-output-schema.json
slug: well-architected-tool-create-workload-output
source_filename: well-architected-tool-create-workload-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    },\n    \"WorkloadArn\": {\n      \"$ref\": \"#/components/schemas/WorkloadArn\"\n    }\n  },\n  \"description\": \"Output of a create workload call.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateWorkloadOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-workload-output-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-workload-output-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: CreateWorkloadOutput
---
