---
description: Returns the number of compliant and noncompliant rules for one or more accounts and regions in an aggregator.
layout: schema
name: AggregateComplianceCount
properties_list:
- description: ''
  name: GroupName
  type: object
- description: ''
  name: ComplianceSummary
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-aggregate-compliance-count-schema.json
slug: config-aggregate-compliance-count
source_filename: config-aggregate-compliance-count-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-compliance-count-schema.json\",\n  \"title\": \"AggregateComplianceCount\",\n  \"description\": \"Returns the number of compliant and noncompliant rules for one or more accounts and regions in an aggregator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The 12-digit account ID or region based on the GroupByKey value.\"\n        }\n      ]\n    },\n    \"ComplianceSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceSummary\"\n        },\n        {\n          \"description\": \"The number of compliant and noncompliant Config rules.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-compliance-count-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: AggregateComplianceCount
---
