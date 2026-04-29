---
description: An infrastructure as code defined resource output.
layout: schema
name: Output
properties_list:
- description: ''
  name: key
  type: object
- description: ''
  name: valueString
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-output-schema.json
slug: amazon-proton-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-output-schema.json\",\n  \"title\": \"Output\",\n  \"description\": \"An infrastructure as code defined resource output.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputKey\"\n        },\n        {\n          \"description\": \"The output key.\"\n        }\n      ]\n    },\n    \"valueString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputValueString\"\n        },\n        {\n          \"description\": \"The output value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: Output
---
