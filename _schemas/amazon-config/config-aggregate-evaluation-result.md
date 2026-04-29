---
description: The details of an Config evaluation for an account ID and region in an aggregator. Provides the Amazon Web Services resource that was evaluated, the compliance of the resource, related time stamps, and supplementary information.
layout: schema
name: AggregateEvaluationResult
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
  name: AccountId
  type: object
- description: ''
  name: AwsRegion
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-aggregate-evaluation-result-schema.json
slug: config-aggregate-evaluation-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-evaluation-result-schema.json\",\n  \"title\": \"AggregateEvaluationResult\",\n  \"description\": \"The details of an Config evaluation for an account ID and region in an aggregator. Provides the Amazon Web Services resource that was evaluated, the compliance of the resource, related time stamps, and supplementary information. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EvaluationResultIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationResultIdentifier\"\n        },\n        {\n          \"description\": \"Uniquely identifies the evaluation result.\"\n        }\n      ]\n    },\n    \"ComplianceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceType\"\n        },\n        {\n      \
  \    \"description\": \"<p>The resource compliance status.</p> <p>For the <code>AggregationEvaluationResult</code> data type, Config supports only the <code>COMPLIANT</code> and <code>NON_COMPLIANT</code>. Config does not support the <code>NOT_APPLICABLE</code> and <code>INSUFFICIENT_DATA</code> value.</p>\"\n        }\n      ]\n    },\n    \"ResultRecordedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time when Config recorded the aggregate evaluation result.\"\n        }\n      ]\n    },\n    \"ConfigRuleInvokedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time when the Config rule evaluated the Amazon Web Services resource.\"\n        }\n      ]\n    },\n    \"Annotation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n     \
  \   },\n        {\n          \"description\": \"Supplementary information about how the agrregate evaluation determined the compliance.\"\n        }\n      ]\n    },\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of the source account.\"\n        }\n      ]\n    },\n    \"AwsRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The source region from where the data is aggregated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-evaluation-result-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: AggregateEvaluationResult
---
