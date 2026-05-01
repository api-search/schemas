---
description: CreateLensVersionInput schema from AWS Well-Architected Tool API
layout: schema
name: CreateLensVersionInput
properties_list:
- description: ''
  name: LensVersion
  type: object
- description: ''
  name: IsMajorVersion
  type: object
- description: ''
  name: ClientRequestToken
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-create-lens-version-input-schema.json
slug: well-architected-tool-create-lens-version-input
source_filename: well-architected-tool-create-lens-version-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"LensVersion\",\n    \"ClientRequestToken\"\n  ],\n  \"title\": \"CreateLensVersionInput\",\n  \"properties\": {\n    \"LensVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensVersion\"\n        },\n        {\n          \"description\": \"The version of the lens being created.\"\n        }\n      ]\n    },\n    \"IsMajorVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IsMajorVersion\"\n        },\n        {\n          \"description\": \"Set to true if this new major lens version.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"$ref\": \"#/components/schemas/ClientRequestToken\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-lens-version-input-schema.json\"\
  ,\n  \"description\": \"CreateLensVersionInput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-lens-version-input-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: CreateLensVersionInput
---
