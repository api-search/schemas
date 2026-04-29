---
description: DeleteEnvironmentTemplateInput schema from Amazon Proton API
layout: schema
name: DeleteEnvironmentTemplateInput
properties_list:
- description: ''
  name: name
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-delete-environment-template-input-schema.json
slug: amazon-proton-delete-environment-template-input
source_filename: amazon-proton-delete-environment-template-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-environment-template-input-schema.json\",\n  \"title\": \"DeleteEnvironmentTemplateInput\",\n  \"description\": \"DeleteEnvironmentTemplateInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the environment template to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-environment-template-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: DeleteEnvironmentTemplateInput
---
