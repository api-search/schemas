---
description: Provides a summary of compliance based on either account ID or region.
layout: schema
name: AggregateConformancePackComplianceSummary
properties_list:
- description: ''
  name: ComplianceSummary
  type: object
- description: ''
  name: GroupName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-aggregate-conformance-pack-compliance-summary-schema.json
slug: config-aggregate-conformance-pack-compliance-summary
source_filename: config-aggregate-conformance-pack-compliance-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-conformance-pack-compliance-summary-schema.json\",\n  \"title\": \"AggregateConformancePackComplianceSummary\",\n  \"description\": \"Provides a summary of compliance based on either account ID or region. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ComplianceSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregateConformancePackComplianceCount\"\n        },\n        {\n          \"description\": \"Returns an <code>AggregateConformancePackComplianceCount</code> object. \"\n        }\n      ]\n    },\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"Groups the result based on Amazon Web Services account ID or Amazon\
  \ Web Services Region.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-conformance-pack-compliance-summary-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: AggregateConformancePackComplianceSummary
---
