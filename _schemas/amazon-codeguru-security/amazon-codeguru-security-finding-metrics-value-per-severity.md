---
description: The severity of the issue in the code that generated a finding.
layout: schema
name: FindingMetricsValuePerSeverity
properties_list:
- description: ''
  name: critical
  type: object
- description: ''
  name: high
  type: object
- description: ''
  name: info
  type: object
- description: ''
  name: low
  type: object
- description: ''
  name: medium
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-finding-metrics-value-per-severity-schema.json
slug: amazon-codeguru-security-finding-metrics-value-per-severity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-finding-metrics-value-per-severity-schema.json\",\n  \"title\": \"FindingMetricsValuePerSeverity\",\n  \"description\": \"The severity of the issue in the code that generated a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"critical\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The severity of the finding is critical and should be addressed immediately.\"\n        }\n      ]\n    },\n    \"high\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The severity of the finding is high and should be addressed as a near-term priority.\"\n        }\n      ]\n    },\n    \"info\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The finding is related to quality or readability improvements and not considered actionable.\"\n        }\n      ]\n    },\n    \"low\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The severity of the finding is low and does require action on its own.\"\n        }\n      ]\n    },\n    \"medium\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The severity of the finding is medium and should be addressed as a mid-term priority.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-finding-metrics-value-per-severity-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: FindingMetricsValuePerSeverity
---
