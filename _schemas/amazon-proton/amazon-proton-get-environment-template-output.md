---
description: GetEnvironmentTemplateOutput schema from Amazon Proton API
layout: schema
name: GetEnvironmentTemplateOutput
properties_list:
- description: ''
  name: environmentTemplate
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-environment-template-output-schema.json
slug: amazon-proton-get-environment-template-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-environment-template-output-schema.json\",\n  \"title\": \"GetEnvironmentTemplateOutput\",\n  \"description\": \"GetEnvironmentTemplateOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentTemplate\"\n        },\n        {\n          \"description\": \"The detailed data of the requested environment template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"environmentTemplate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-environment-template-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetEnvironmentTemplateOutput
---
