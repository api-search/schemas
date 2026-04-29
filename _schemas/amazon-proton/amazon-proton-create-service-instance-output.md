---
description: CreateServiceInstanceOutput schema from Amazon Proton API
layout: schema
name: CreateServiceInstanceOutput
properties_list:
- description: ''
  name: serviceInstance
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-create-service-instance-output-schema.json
slug: amazon-proton-create-service-instance-output
source_filename: amazon-proton-create-service-instance-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-service-instance-output-schema.json\",\n  \"title\": \"CreateServiceInstanceOutput\",\n  \"description\": \"CreateServiceInstanceOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceInstance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceInstance\"\n        },\n        {\n          \"description\": \"The detailed data of the service instance being created.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"serviceInstance\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-create-service-instance-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CreateServiceInstanceOutput
---
