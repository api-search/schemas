---
description: The list of Amazon Web Services Regions associated with the workload, for example, <code>us-east-2</code>, or <code>ca-central-1</code>.
layout: schema
name: WorkloadAwsRegions
properties_list: []
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-workload-aws-regions-schema.json
slug: well-architected-tool-workload-aws-regions
source_filename: well-architected-tool-workload-aws-regions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"description\": \"The list of Amazon Web Services Regions associated with the workload, for example, <code>us-east-2</code>, or <code>ca-central-1</code>.\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/AwsRegion\"\n  },\n  \"maxItems\": 50,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkloadAwsRegions\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-aws-regions-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-aws-regions-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: WorkloadAwsRegions
---
