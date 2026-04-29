---
description: A pillar difference return object.
layout: schema
name: PillarDifference
properties_list:
- description: ''
  name: PillarId
  type: object
- description: ''
  name: PillarName
  type: object
- description: ''
  name: DifferenceStatus
  type: object
- description: ''
  name: QuestionDifferences
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-pillar-difference-schema.json
slug: well-architected-tool-pillar-difference
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"PillarId\": {\n      \"$ref\": \"#/components/schemas/PillarId\"\n    },\n    \"PillarName\": {\n      \"$ref\": \"#/components/schemas/PillarName\"\n    },\n    \"DifferenceStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DifferenceStatus\"\n        },\n        {\n          \"description\": \"Indicates the type of change to the pillar.\"\n        }\n      ]\n    },\n    \"QuestionDifferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QuestionDifferences\"\n        },\n        {\n          \"description\": \"List of question differences.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A pillar difference return object.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PillarDifference\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-pillar-difference-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-pillar-difference-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: PillarDifference
---
