---
description: The details of a conformance pack evaluation. Provides Config rule and Amazon Web Services resource type that was evaluated, the compliance of the conformance pack, related time stamps, and supplementary information.
layout: schema
name: ConformancePackEvaluationResult
properties_list:
- description: ''
  name: ComplianceType
  type: object
- description: ''
  name: EvaluationResultIdentifier
  type: object
- description: ''
  name: ConfigRuleInvokedTime
  type: object
- description: ''
  name: ResultRecordedTime
  type: object
- description: ''
  name: Annotation
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-conformance-pack-evaluation-result-schema.json
slug: config-conformance-pack-evaluation-result
source_filename: config-conformance-pack-evaluation-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-evaluation-result-schema.json\",\n  \"title\": \"ConformancePackEvaluationResult\",\n  \"description\": \"The details of a conformance pack evaluation. Provides Config rule and Amazon Web Services resource type that was evaluated, the compliance of the conformance pack, related time stamps, and supplementary information. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ComplianceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackComplianceType\"\n        },\n        {\n          \"description\": \"The compliance type. The allowed values are <code>COMPLIANT</code> and <code>NON_COMPLIANT</code>. <code>INSUFFICIENT_DATA</code> is not supported.\"\n        }\n      ]\n    },\n    \"EvaluationResultIdentifier\": {\n      \"$ref\"\
  : \"#/components/schemas/EvaluationResultIdentifier\"\n    },\n    \"ConfigRuleInvokedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time when Config rule evaluated Amazon Web Services resource.\"\n        }\n      ]\n    },\n    \"ResultRecordedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time when Config recorded the evaluation result. \"\n        }\n      ]\n    },\n    \"Annotation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Annotation\"\n        },\n        {\n          \"description\": \"Supplementary information about how the evaluation determined the compliance. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ComplianceType\",\n    \"EvaluationResultIdentifier\",\n    \"ConfigRuleInvokedTime\",\n    \"ResultRecordedTime\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-evaluation-result-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ConformancePackEvaluationResult
---
