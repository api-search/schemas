---
description: GetConsolidatedReportOutput schema from AWS Well-Architected Tool API
layout: schema
name: GetConsolidatedReportOutput
properties_list:
- description: ''
  name: Metrics
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Base64String
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-get-consolidated-report-output-schema.json
slug: well-architected-tool-get-consolidated-report-output
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Metrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConsolidatedReportMetrics\"\n        },\n        {\n          \"description\": \"<p>The metrics that make up the consolidated report.</p> <p>Only returned when <code>JSON</code> format is requested.</p>\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    },\n    \"Base64String\": {\n      \"$ref\": \"#/components/schemas/Base64String\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetConsolidatedReportOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-consolidated-report-output-schema.json\",\n  \"description\": \"GetConsolidatedReportOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-consolidated-report-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: GetConsolidatedReportOutput
---
