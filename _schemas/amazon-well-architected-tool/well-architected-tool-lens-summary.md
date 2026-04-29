---
description: A lens summary of a lens.
layout: schema
name: LensSummary
properties_list:
- description: ''
  name: LensArn
  type: object
- description: ''
  name: LensAlias
  type: object
- description: ''
  name: LensName
  type: object
- description: ''
  name: LensType
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: UpdatedAt
  type: object
- description: ''
  name: LensVersion
  type: object
- description: ''
  name: Owner
  type: object
- description: ''
  name: LensStatus
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-lens-summary-schema.json
slug: well-architected-tool-lens-summary
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LensArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"The ARN of the lens.\"\n        }\n      ]\n    },\n    \"LensAlias\": {\n      \"$ref\": \"#/components/schemas/LensAlias\"\n    },\n    \"LensName\": {\n      \"$ref\": \"#/components/schemas/LensName\"\n    },\n    \"LensType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensType\"\n        },\n        {\n          \"description\": \"The type of the lens.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"$ref\": \"#/components/schemas/LensDescription\"\n    },\n    \"CreatedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"UpdatedAt\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"LensVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensVersion\"\
  \n        },\n        {\n          \"description\": \"The version of the lens.\"\n        }\n      ]\n    },\n    \"Owner\": {\n      \"$ref\": \"#/components/schemas/AwsAccountId\"\n    },\n    \"LensStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensStatus\"\n        },\n        {\n          \"description\": \"The status of the lens.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A lens summary of a lens.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LensSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-lens-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-lens-summary-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: LensSummary
---
