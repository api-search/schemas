---
description: GetServiceInstanceInput schema from Amazon Proton API
layout: schema
name: GetServiceInstanceInput
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: serviceName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-service-instance-input-schema.json
slug: amazon-proton-get-service-instance-input
source_filename: amazon-proton-get-service-instance-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-service-instance-input-schema.json\",\n  \"title\": \"GetServiceInstanceInput\",\n  \"description\": \"GetServiceInstanceInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of a service instance that you want to get the detailed data for.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service that you want the service instance input for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"serviceName\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-service-instance-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetServiceInstanceInput
---
