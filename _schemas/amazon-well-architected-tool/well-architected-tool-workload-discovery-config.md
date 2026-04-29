---
description: Discovery configuration associated to the workload.
layout: schema
name: WorkloadDiscoveryConfig
properties_list:
- description: ''
  name: TrustedAdvisorIntegrationStatus
  type: object
- description: ''
  name: WorkloadResourceDefinition
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-workload-discovery-config-schema.json
slug: well-architected-tool-workload-discovery-config
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"TrustedAdvisorIntegrationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrustedAdvisorIntegrationStatus\"\n        },\n        {\n          \"description\": \"Discovery integration status in respect to Trusted Advisor for the workload.\"\n        }\n      ]\n    },\n    \"WorkloadResourceDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkloadResourceDefinition\"\n        },\n        {\n          \"description\": \"<p>The mode to use for identifying resources associated with the workload.</p> <p>You can specify <code>WORKLOAD_METADATA</code>, <code>APP_REGISTRY</code>, or both.</p>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Discovery configuration associated to the workload.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkloadDiscoveryConfig\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-discovery-config-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-workload-discovery-config-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: WorkloadDiscoveryConfig
---
