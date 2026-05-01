---
description: Account details for a Well-Architected best practice in relation to Trusted Advisor checks.
layout: schema
name: CheckDetail
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Provider
  type: object
- description: ''
  name: LensArn
  type: object
- description: ''
  name: PillarId
  type: object
- description: ''
  name: QuestionId
  type: object
- description: ''
  name: ChoiceId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: AccountId
  type: object
- description: ''
  name: FlaggedResources
  type: object
- description: ''
  name: Reason
  type: object
- description: ''
  name: UpdatedAt
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-check-detail-schema.json
slug: well-architected-tool-check-detail
source_filename: well-architected-tool-check-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckId\"\n        },\n        {\n          \"description\": \"Trusted Advisor check ID.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckName\"\n        },\n        {\n          \"description\": \"Trusted Advisor check name.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckDescription\"\n        },\n        {\n          \"description\": \"Trusted Advisor check description.\"\n        }\n      ]\n    },\n    \"Provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckProvider\"\n        },\n        {\n          \"description\": \"Provider of the check related to the best practice.\"\n        }\n      ]\n    },\n    \"LensArn\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"Well-Architected Lens ARN associated to the check.\"\n        }\n      ]\n    },\n    \"PillarId\": {\n      \"$ref\": \"#/components/schemas/PillarId\"\n    },\n    \"QuestionId\": {\n      \"$ref\": \"#/components/schemas/QuestionId\"\n    },\n    \"ChoiceId\": {\n      \"$ref\": \"#/components/schemas/ChoiceId\"\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckStatus\"\n        },\n        {\n          \"description\": \"Status associated to the check.\"\n        }\n      ]\n    },\n    \"AccountId\": {\n      \"$ref\": \"#/components/schemas/AwsAccountId\"\n    },\n    \"FlaggedResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlaggedResources\"\n        },\n        {\n          \"description\": \"Count of flagged resources associated to the check.\"\n        }\n  \
  \    ]\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckFailureReason\"\n        },\n        {\n          \"description\": \"Reason associated to the check.\"\n        }\n      ]\n    },\n    \"UpdatedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    }\n  },\n  \"description\": \"Account details for a Well-Architected best practice in relation to Trusted Advisor checks.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CheckDetail\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-check-detail-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-check-detail-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: CheckDetail
---
