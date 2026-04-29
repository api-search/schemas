---
description: The number of Amazon Web Services resources of a specific type that are compliant or noncompliant, up to a maximum of 100 for each.
layout: schema
name: ComplianceSummaryByResourceType
properties_list:
- description: ''
  name: ResourceType
  type: object
- description: ''
  name: ComplianceSummary
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-compliance-summary-by-resource-type-schema.json
slug: config-compliance-summary-by-resource-type
source_filename: config-compliance-summary-by-resource-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-compliance-summary-by-resource-type-schema.json\",\n  \"title\": \"ComplianceSummaryByResourceType\",\n  \"description\": \"The number of Amazon Web Services resources of a specific type that are compliant or noncompliant, up to a maximum of 100 for each.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The type of Amazon Web Services resource.\"\n        }\n      ]\n    },\n    \"ComplianceSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceSummary\"\n        },\n        {\n          \"description\": \"The number of Amazon Web Services resources that are compliant or noncompliant,\
  \ up to a maximum of 100 for each.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-compliance-summary-by-resource-type-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ComplianceSummaryByResourceType
---
