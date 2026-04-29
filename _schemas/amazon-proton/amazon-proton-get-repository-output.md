---
description: GetRepositoryOutput schema from Amazon Proton API
layout: schema
name: GetRepositoryOutput
properties_list:
- description: ''
  name: repository
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-repository-output-schema.json
slug: amazon-proton-get-repository-output
source_filename: amazon-proton-get-repository-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-repository-output-schema.json\",\n  \"title\": \"GetRepositoryOutput\",\n  \"description\": \"GetRepositoryOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Repository\"\n        },\n        {\n          \"description\": \"The repository link's detail data that's returned by Proton.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"repository\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-repository-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetRepositoryOutput
---
