---
description: Trusted Advisor check summary.
layout: schema
name: CheckSummary
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Provider
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: UpdatedAt
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
  name: AccountSummary
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-check-summary-schema.json
slug: well-architected-tool-check-summary
source_filename: well-architected-tool-check-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckId\"\n        },\n        {\n          \"description\": \"Trusted Advisor check ID.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckName\"\n        },\n        {\n          \"description\": \"Trusted Advisor check name.\"\n        }\n      ]\n    },\n    \"Provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckProvider\"\n        },\n        {\n          \"description\": \"Provider of the check related to the best practice.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckDescription\"\n        },\n        {\n          \"description\": \"Trusted Advisor check description.\"\n        }\n      ]\n    },\n    \"UpdatedAt\": {\n      \"$ref\"\
  : \"#/components/schemas/Timestamp\"\n    },\n    \"LensArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"Well-Architected Lens ARN associated to the check.\"\n        }\n      ]\n    },\n    \"PillarId\": {\n      \"$ref\": \"#/components/schemas/PillarId\"\n    },\n    \"QuestionId\": {\n      \"$ref\": \"#/components/schemas/QuestionId\"\n    },\n    \"ChoiceId\": {\n      \"$ref\": \"#/components/schemas/ChoiceId\"\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckStatus\"\n        },\n        {\n          \"description\": \"Status associated to the check.\"\n        }\n      ]\n    },\n    \"AccountSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountSummary\"\n        },\n        {\n          \"description\": \"Account summary associated to the check.\"\n        }\n      ]\n    }\n  },\n\
  \  \"description\": \"Trusted Advisor check summary.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CheckSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-check-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-check-summary-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: CheckSummary
---
