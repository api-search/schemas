---
description: DeleteServiceOutput schema from Amazon Proton API
layout: schema
name: DeleteServiceOutput
properties_list:
- description: ''
  name: service
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-delete-service-output-schema.json
slug: amazon-proton-delete-service-output
source_filename: amazon-proton-delete-service-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-service-output-schema.json\",\n  \"title\": \"DeleteServiceOutput\",\n  \"description\": \"DeleteServiceOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Service\"\n        },\n        {\n          \"description\": \"The detailed data of the service being deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-service-output-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: DeleteServiceOutput
---
