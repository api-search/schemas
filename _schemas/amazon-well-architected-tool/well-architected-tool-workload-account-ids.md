---
description: The list of Amazon Web Services account IDs associated with the workload.
layout: schema
name: WorkloadAccountIds
properties_list: []
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-workload-account-ids-schema.json
slug: well-architected-tool-workload-account-ids
source_filename: well-architected-tool-workload-account-ids-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"description\": \"The list of Amazon Web Services account IDs associated with the workload.\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/AwsAccountId\"\n  },\n  \"maxItems\": 100,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkloadAccountIds\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-account-ids-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-account-ids-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: WorkloadAccountIds
---
