---
description: The details of an Config evaluation. Provides the Amazon Web Services resource that was evaluated, the compliance of the resource, related time stamps, and supplementary information.
layout: schema
name: EvaluationResult
properties_list:
- description: ''
  name: EvaluationResultIdentifier
  type: object
- description: ''
  name: ComplianceType
  type: object
- description: ''
  name: ResultRecordedTime
  type: object
- description: ''
  name: ConfigRuleInvokedTime
  type: object
- description: ''
  name: Annotation
  type: object
- description: ''
  name: ResultToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-evaluation-result-schema.json
slug: config-evaluation-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-evaluation-result-schema.json\",\n  \"title\": \"EvaluationResult\",\n  \"description\": \"The details of an Config evaluation. Provides the Amazon Web Services resource that was evaluated, the compliance of the resource, related time stamps, and supplementary information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EvaluationResultIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationResultIdentifier\"\n        },\n        {\n          \"description\": \"Uniquely identifies the evaluation result.\"\n        }\n      ]\n    },\n    \"ComplianceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceType\"\n        },\n        {\n          \"description\": \"<p>Indicates whether the Amazon Web Services\
  \ resource complies with the Config rule that evaluated it.</p> <p>For the <code>EvaluationResult</code> data type, Config supports only the <code>COMPLIANT</code>, <code>NON_COMPLIANT</code>, and <code>NOT_APPLICABLE</code> values. Config does not support the <code>INSUFFICIENT_DATA</code> value for the <code>EvaluationResult</code> data type.</p>\"\n        }\n      ]\n    },\n    \"ResultRecordedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time when Config recorded the evaluation result.\"\n        }\n      ]\n    },\n    \"ConfigRuleInvokedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time when the Config rule evaluated the Amazon Web Services resource.\"\n        }\n      ]\n    },\n    \"Annotation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\
  \n        },\n        {\n          \"description\": \"Supplementary information about how the evaluation determined the compliance.\"\n        }\n      ]\n    },\n    \"ResultToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An encrypted token that associates an evaluation with an Config rule. The token identifies the rule, the Amazon Web Services resource being evaluated, and the event that triggered the evaluation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-evaluation-result-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: EvaluationResult
---
