---
description: Information about summary metrics in an account.
layout: schema
name: MetricsSummary
properties_list:
- description: ''
  name: categoriesWithMostFindings
  type: object
- description: ''
  name: date
  type: object
- description: ''
  name: openFindings
  type: object
- description: ''
  name: scansWithMostOpenCriticalFindings
  type: object
- description: ''
  name: scansWithMostOpenFindings
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-metrics-summary-schema.json
slug: amazon-codeguru-security-metrics-summary
source_filename: amazon-codeguru-security-metrics-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-metrics-summary-schema.json\",\n  \"title\": \"MetricsSummary\",\n  \"description\": \"Information about summary metrics in an account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"categoriesWithMostFindings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CategoriesWithMostFindings\"\n        },\n        {\n          \"description\": \"A list of <code>CategoryWithFindingNum</code> objects for the top 5 finding categories with the most open findings in an account.\"\n        }\n      ]\n    },\n    \"date\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date from which the metrics summary information was retrieved.\"\n        }\n\
  \      ]\n    },\n    \"openFindings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingMetricsValuePerSeverity\"\n        },\n        {\n          \"description\": \"The number of open findings of each severity in an account.\"\n        }\n      ]\n    },\n    \"scansWithMostOpenCriticalFindings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScansWithMostOpenCriticalFindings\"\n        },\n        {\n          \"description\": \"A list of <code>ScanNameWithFindingNum</code> objects for the top 3 scans with the most number of open findings in an account.\"\n        }\n      ]\n    },\n    \"scansWithMostOpenFindings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScansWithMostOpenFindings\"\n        },\n        {\n          \"description\": \"A list of <code>ScanNameWithFindingNum</code> objects for the top 3 scans with the most number of open critical findings in an account.\"\n      \
  \  }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-metrics-summary-schema.json
tags:
- Amazon
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: MetricsSummary
---
