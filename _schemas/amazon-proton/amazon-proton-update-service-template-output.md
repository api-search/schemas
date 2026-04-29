---
description: UpdateServiceTemplateOutput schema from Amazon Proton API
layout: schema
name: UpdateServiceTemplateOutput
properties_list:
- description: ''
  name: serviceTemplate
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-service-template-output-schema.json
slug: amazon-proton-update-service-template-output
source_filename: amazon-proton-update-service-template-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-template-output-schema.json\",\n  \"title\": \"UpdateServiceTemplateOutput\",\n  \"description\": \"UpdateServiceTemplateOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceTemplate\"\n        },\n        {\n          \"description\": \"The service template detail data that's returned by Proton.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceTemplate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-template-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateServiceTemplateOutput
---
