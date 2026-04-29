---
description: A metric that contributes to the consolidated report.
layout: schema
name: ConsolidatedReportMetric
properties_list:
- description: ''
  name: MetricType
  type: object
- description: ''
  name: RiskCounts
  type: object
- description: ''
  name: WorkloadId
  type: object
- description: ''
  name: WorkloadName
  type: object
- description: ''
  name: WorkloadArn
  type: object
- description: ''
  name: UpdatedAt
  type: object
- description: ''
  name: Lenses
  type: object
- description: ''
  name: LensesAppliedCount
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-consolidated-report-metric-schema.json
slug: well-architected-tool-consolidated-report-metric
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricType\"\n        },\n        {\n          \"description\": \"The metric type of a metric in the consolidated report. Currently only WORKLOAD metric types are supported.\"\n        }\n      ]\n    },\n    \"RiskCounts\": {\n      \"$ref\": \"#/components/schemas/RiskCounts\"\n    },\n    \"WorkloadId\": {\n      \"$ref\": \"#/components/schemas/WorkloadId\"\n    },\n    \"WorkloadName\": {\n      \"$ref\": \"#/components/schemas/WorkloadName\"\n    },\n    \"WorkloadArn\": {\n      \"$ref\": \"#/components/schemas/WorkloadArn\"\n    },\n    \"UpdatedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"Lenses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensMetrics\"\n        },\n        {\n          \"description\": \"The metrics for the lenses in the workload.\"\n     \
  \   }\n      ]\n    },\n    \"LensesAppliedCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensesAppliedCount\"\n        },\n        {\n          \"description\": \"The total number of lenses applied to the workload.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A metric that contributes to the consolidated report.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConsolidatedReportMetric\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-consolidated-report-metric-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-consolidated-report-metric-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ConsolidatedReportMetric
---
