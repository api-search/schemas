---
description: UpdateEnvironmentTemplateVersionOutput schema from Amazon Proton API
layout: schema
name: UpdateEnvironmentTemplateVersionOutput
properties_list:
- description: ''
  name: environmentTemplateVersion
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-environment-template-version-output-schema.json
slug: amazon-proton-update-environment-template-version-output
source_filename: amazon-proton-update-environment-template-version-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-environment-template-version-output-schema.json\",\n  \"title\": \"UpdateEnvironmentTemplateVersionOutput\",\n  \"description\": \"UpdateEnvironmentTemplateVersionOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentTemplateVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentTemplateVersion\"\n        },\n        {\n          \"description\": \"The environment template version detail data that's returned by Proton.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"environmentTemplateVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-environment-template-version-output-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateEnvironmentTemplateVersionOutput
---
