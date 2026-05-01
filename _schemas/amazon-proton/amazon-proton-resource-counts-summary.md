---
description: Summary counts of each Proton resource types.
layout: schema
name: ResourceCountsSummary
properties_list:
- description: ''
  name: behindMajor
  type: object
- description: ''
  name: behindMinor
  type: object
- description: ''
  name: failed
  type: object
- description: ''
  name: total
  type: object
- description: ''
  name: upToDate
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-resource-counts-summary-schema.json
slug: amazon-proton-resource-counts-summary
source_filename: amazon-proton-resource-counts-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-resource-counts-summary-schema.json\",\n  \"title\": \"ResourceCountsSummary\",\n  \"description\": \"Summary counts of each Proton resource types.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"behindMajor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of resources of this type in the Amazon Web Services account that need a major template version update.\"\n        }\n      ]\n    },\n    \"behindMinor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of resources of this type in the Amazon Web Services account that need a minor template version update.\"\n        }\n     \
  \ ]\n    },\n    \"failed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of resources of this type in the Amazon Web Services account that failed to deploy.\"\n        }\n      ]\n    },\n    \"total\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The total number of resources of this type in the Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"upToDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of resources of this type in the Amazon Web Services account that are up-to-date with their template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"total\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-resource-counts-summary-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ResourceCountsSummary
---
