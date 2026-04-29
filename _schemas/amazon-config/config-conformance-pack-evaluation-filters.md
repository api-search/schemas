---
description: Filters a conformance pack by Config rule names, compliance types, Amazon Web Services resource types, and resource IDs.
layout: schema
name: ConformancePackEvaluationFilters
properties_list:
- description: ''
  name: ConfigRuleNames
  type: object
- description: ''
  name: ComplianceType
  type: object
- description: ''
  name: ResourceType
  type: object
- description: ''
  name: ResourceIds
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-conformance-pack-evaluation-filters-schema.json
slug: config-conformance-pack-evaluation-filters
source_filename: config-conformance-pack-evaluation-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-evaluation-filters-schema.json\",\n  \"title\": \"ConformancePackEvaluationFilters\",\n  \"description\": \"Filters a conformance pack by Config rule names, compliance types, Amazon Web Services resource types, and resource IDs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackConfigRuleNames\"\n        },\n        {\n          \"description\": \"Filters the results by Config rule names.\"\n        }\n      ]\n    },\n    \"ComplianceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackComplianceType\"\n        },\n        {\n          \"description\": \"<p>Filters the results by compliance.</p> <p>The allowed values are\
  \ <code>COMPLIANT</code> and <code>NON_COMPLIANT</code>. <code>INSUFFICIENT_DATA</code> is not supported.</p>\"\n        }\n      ]\n    },\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"Filters the results by the resource type (for example, <code>\\\"AWS::EC2::Instance\\\"</code>). \"\n        }\n      ]\n    },\n    \"ResourceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackComplianceResourceIds\"\n        },\n        {\n          \"description\": \"<p>Filters the results by resource IDs.</p> <note> <p>This is valid only when you provide resource type. If there is no resource type, you will see an error.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-evaluation-filters-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ConformancePackEvaluationFilters
---
