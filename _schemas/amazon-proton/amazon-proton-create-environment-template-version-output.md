---
description: CreateEnvironmentTemplateVersionOutput schema from Amazon Proton API
layout: schema
name: CreateEnvironmentTemplateVersionOutput
properties_list:
- description: ''
  name: environmentTemplateVersion
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-create-environment-template-version-output-schema.json
slug: amazon-proton-create-environment-template-version-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-environment-template-version-output-schema.json\",\n  \"title\": \"CreateEnvironmentTemplateVersionOutput\",\n  \"description\": \"CreateEnvironmentTemplateVersionOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentTemplateVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentTemplateVersion\"\n        },\n        {\n          \"description\": \"The environment template detail data that's returned by Proton.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"environmentTemplateVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-environment-template-version-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CreateEnvironmentTemplateVersionOutput
---
