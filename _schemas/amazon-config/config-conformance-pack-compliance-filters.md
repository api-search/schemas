---
description: Filters the conformance pack by compliance types and Config rule names.
layout: schema
name: ConformancePackComplianceFilters
properties_list:
- description: ''
  name: ConfigRuleNames
  type: object
- description: ''
  name: ComplianceType
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-conformance-pack-compliance-filters-schema.json
slug: config-conformance-pack-compliance-filters
source_filename: config-conformance-pack-compliance-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-compliance-filters-schema.json\",\n  \"title\": \"ConformancePackComplianceFilters\",\n  \"description\": \"Filters the conformance pack by compliance types and Config rule names.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackConfigRuleNames\"\n        },\n        {\n          \"description\": \"Filters the results by Config rule names.\"\n        }\n      ]\n    },\n    \"ComplianceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackComplianceType\"\n        },\n        {\n          \"description\": \"<p>Filters the results by compliance.</p> <p>The allowed values are <code>COMPLIANT</code> and <code>NON_COMPLIANT</code>.\
  \ <code>INSUFFICIENT_DATA</code> is not supported.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-compliance-filters-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ConformancePackComplianceFilters
---
