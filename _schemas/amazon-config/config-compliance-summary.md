---
description: The number of Config rules or Amazon Web Services resources that are compliant and noncompliant.
layout: schema
name: ComplianceSummary
properties_list:
- description: ''
  name: CompliantResourceCount
  type: object
- description: ''
  name: NonCompliantResourceCount
  type: object
- description: ''
  name: ComplianceSummaryTimestamp
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-compliance-summary-schema.json
slug: config-compliance-summary
source_filename: config-compliance-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-compliance-summary-schema.json\",\n  \"title\": \"ComplianceSummary\",\n  \"description\": \"The number of Config rules or Amazon Web Services resources that are compliant and noncompliant.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CompliantResourceCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceContributorCount\"\n        },\n        {\n          \"description\": \"The number of Config rules or Amazon Web Services resources that are compliant, up to a maximum of 25 for rules and 100 for resources.\"\n        }\n      ]\n    },\n    \"NonCompliantResourceCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceContributorCount\"\n        },\n        {\n          \"description\": \"The number of Config\
  \ rules or Amazon Web Services resources that are noncompliant, up to a maximum of 25 for rules and 100 for resources.\"\n        }\n      ]\n    },\n    \"ComplianceSummaryTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time that Config created the compliance summary.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-compliance-summary-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ComplianceSummary
---
