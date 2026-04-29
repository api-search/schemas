---
description: GetResourcesSummaryOutput schema from Amazon Proton API
layout: schema
name: GetResourcesSummaryOutput
properties_list:
- description: ''
  name: counts
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-resources-summary-output-schema.json
slug: amazon-proton-get-resources-summary-output
source_filename: amazon-proton-get-resources-summary-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-resources-summary-output-schema.json\",\n  \"title\": \"GetResourcesSummaryOutput\",\n  \"description\": \"GetResourcesSummaryOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"counts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountsSummary\"\n        },\n        {\n          \"description\": \"Summary counts of each Proton resource type.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"counts\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-resources-summary-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetResourcesSummaryOutput
---
