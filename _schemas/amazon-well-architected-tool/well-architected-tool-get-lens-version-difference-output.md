---
description: GetLensVersionDifferenceOutput schema from AWS Well-Architected Tool API
layout: schema
name: GetLensVersionDifferenceOutput
properties_list:
- description: ''
  name: LensAlias
  type: object
- description: ''
  name: LensArn
  type: object
- description: ''
  name: BaseLensVersion
  type: object
- description: ''
  name: TargetLensVersion
  type: object
- description: ''
  name: LatestLensVersion
  type: object
- description: ''
  name: VersionDifferences
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-get-lens-version-difference-output-schema.json
slug: well-architected-tool-get-lens-version-difference-output
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LensAlias\": {\n      \"$ref\": \"#/components/schemas/LensAlias\"\n    },\n    \"LensArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"The ARN for the lens.\"\n        }\n      ]\n    },\n    \"BaseLensVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensVersion\"\n        },\n        {\n          \"description\": \"The base version of the lens.\"\n        }\n      ]\n    },\n    \"TargetLensVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensVersion\"\n        },\n        {\n          \"description\": \"The target lens version for the lens.\"\n        }\n      ]\n    },\n    \"LatestLensVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensVersion\"\n        },\n        {\n          \"description\": \"The latest\
  \ version of the lens.\"\n        }\n      ]\n    },\n    \"VersionDifferences\": {\n      \"$ref\": \"#/components/schemas/VersionDifferences\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetLensVersionDifferenceOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-lens-version-difference-output-schema.json\",\n  \"description\": \"GetLensVersionDifferenceOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-lens-version-difference-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: GetLensVersionDifferenceOutput
---
