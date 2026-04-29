---
description: Identifies an Amazon Web Services resource and indicates whether it complies with the Config rule that it was evaluated against.
layout: schema
name: ExternalEvaluation
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
schema_file: json-schema/config-external-evaluation-schema.json
slug: config-external-evaluation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-external-evaluation-schema.json\",\n  \"title\": \"ExternalEvaluation\",\n  \"description\": \"Identifies an Amazon Web Services resource and indicates whether it complies with the Config rule that it was evaluated against.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ComplianceResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The evaluated compliance resource type. Config accepts <code>AWS::::Account</code> resource type.\"\n        }\n      ]\n    },\n    \"ComplianceResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BaseResourceId\"\n        },\n        {\n          \"description\": \"The evaluated compliance resource ID. Config\
  \ accepts only Amazon Web Services account ID.\"\n        }\n      ]\n    },\n    \"ComplianceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceType\"\n        },\n        {\n          \"description\": \"The compliance of the Amazon Web Services resource. The valid values are <code>COMPLIANT, NON_COMPLIANT, </code> and <code>NOT_APPLICABLE</code>.\"\n        }\n      ]\n    },\n    \"Annotation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"Supplementary information about the reason of compliance. For example, this task was completed on a specific date.\"\n        }\n      ]\n    },\n    \"OrderingTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderingTimestamp\"\n        },\n        {\n          \"description\": \"The time when the compliance was recorded. \"\n        }\n      ]\n    }\n \
  \ },\n  \"required\": [\n    \"ComplianceResourceType\",\n    \"ComplianceResourceId\",\n    \"ComplianceType\",\n    \"OrderingTimestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-external-evaluation-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ExternalEvaluation
---
