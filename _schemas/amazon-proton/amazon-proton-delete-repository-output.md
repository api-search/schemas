---
description: DeleteRepositoryOutput schema from Amazon Proton API
layout: schema
name: DeleteRepositoryOutput
properties_list:
- description: ''
  name: repository
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-delete-repository-output-schema.json
slug: amazon-proton-delete-repository-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-repository-output-schema.json\",\n  \"title\": \"DeleteRepositoryOutput\",\n  \"description\": \"DeleteRepositoryOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Repository\"\n        },\n        {\n          \"description\": \"The deleted repository link's detail data that's returned by Proton.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-repository-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: DeleteRepositoryOutput
---
