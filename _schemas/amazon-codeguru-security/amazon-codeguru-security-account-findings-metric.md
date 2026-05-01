---
description: A summary of findings metrics in an account.
layout: schema
name: AccountFindingsMetric
properties_list:
- description: ''
  name: closedFindings
  type: object
- description: ''
  name: date
  type: object
- description: ''
  name: meanTimeToClose
  type: object
- description: ''
  name: newFindings
  type: object
- description: ''
  name: openFindings
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-account-findings-metric-schema.json
slug: amazon-codeguru-security-account-findings-metric
source_filename: amazon-codeguru-security-account-findings-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-account-findings-metric-schema.json\",\n  \"title\": \"AccountFindingsMetric\",\n  \"description\": \"A summary of findings metrics in an account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"closedFindings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingMetricsValuePerSeverity\"\n        },\n        {\n          \"description\": \"The number of closed findings of each severity in an account on the specified date.\"\n        }\n      ]\n    },\n    \"date\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date from which the finding metrics were retrieved.\"\n        }\n      ]\n    },\n    \"meanTimeToClose\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingMetricsValuePerSeverity\"\n        },\n        {\n          \"description\": \"The average time it takes to close findings of each severity in days.\"\n        }\n      ]\n    },\n    \"newFindings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingMetricsValuePerSeverity\"\n        },\n        {\n          \"description\": \"The number of new findings of each severity in account on the specified date.\"\n        }\n      ]\n    },\n    \"openFindings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingMetricsValuePerSeverity\"\n        },\n        {\n          \"description\": \"The number of open findings of each severity in an account as of the specified date.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-account-findings-metric-schema.json
tags:
- Amazon
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: AccountFindingsMetric
---
