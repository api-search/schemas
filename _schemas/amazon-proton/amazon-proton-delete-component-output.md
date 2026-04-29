---
description: DeleteComponentOutput schema from Amazon Proton API
layout: schema
name: DeleteComponentOutput
properties_list:
- description: ''
  name: component
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-delete-component-output-schema.json
slug: amazon-proton-delete-component-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-component-output-schema.json\",\n  \"title\": \"DeleteComponentOutput\",\n  \"description\": \"DeleteComponentOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"component\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Component\"\n        },\n        {\n          \"description\": \"The detailed data of the component being deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-component-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: DeleteComponentOutput
---
