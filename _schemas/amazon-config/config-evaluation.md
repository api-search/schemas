---
description: Identifies an Amazon Web Services resource and indicates whether it complies with the Config rule that it was evaluated against.
layout: schema
name: Evaluation
properties_list:
- description: ''
  name: ComplianceResourceType
  type: object
- description: ''
  name: ComplianceResourceId
  type: object
- description: ''
  name: ComplianceType
  type: object
- description: ''
  name: Annotation
  type: object
- description: ''
  name: OrderingTimestamp
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-evaluation-schema.json
slug: config-evaluation
source_filename: config-evaluation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-evaluation-schema.json\",\n  \"title\": \"Evaluation\",\n  \"description\": \"Identifies an Amazon Web Services resource and indicates whether it complies with the Config rule that it was evaluated against.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ComplianceResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The type of Amazon Web Services resource that was evaluated.\"\n        }\n      ]\n    },\n    \"ComplianceResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BaseResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services resource that was evaluated.\"\n        }\n      ]\n    },\n\
  \    \"ComplianceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceType\"\n        },\n        {\n          \"description\": \"<p>Indicates whether the Amazon Web Services resource complies with the Config rule that it was evaluated against.</p> <p>For the <code>Evaluation</code> data type, Config supports only the <code>COMPLIANT</code>, <code>NON_COMPLIANT</code>, and <code>NOT_APPLICABLE</code> values. Config does not support the <code>INSUFFICIENT_DATA</code> value for this data type.</p> <p>Similarly, Config does not accept <code>INSUFFICIENT_DATA</code> as the value for <code>ComplianceType</code> from a <code>PutEvaluations</code> request. For example, an Lambda function for a custom Config rule cannot pass an <code>INSUFFICIENT_DATA</code> value to Config.</p>\"\n        }\n      ]\n    },\n    \"Annotation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n\
  \          \"description\": \"Supplementary information about how the evaluation determined the compliance.\"\n        }\n      ]\n    },\n    \"OrderingTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderingTimestamp\"\n        },\n        {\n          \"description\": \"The time of the event in Config that triggered the evaluation. For event-based evaluations, the time indicates when Config created the configuration item that triggered the evaluation. For periodic evaluations, the time indicates when Config triggered the evaluation at the frequency that you specified (for example, every 24 hours).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ComplianceResourceType\",\n    \"ComplianceResourceId\",\n    \"ComplianceType\",\n    \"OrderingTimestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-evaluation-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: Evaluation
---
