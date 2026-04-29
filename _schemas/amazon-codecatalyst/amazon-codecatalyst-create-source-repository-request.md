---
description: CreateSourceRepositoryRequest schema from Amazon CodeCatalyst
layout: schema
name: CreateSourceRepositoryRequest
properties_list:
- description: ''
  name: description
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-create-source-repository-request-schema.json
slug: amazon-codecatalyst-create-source-repository-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-source-repository-request-schema.json\",\n  \"title\": \"CreateSourceRepositoryRequest\",\n  \"description\": \"CreateSourceRepositoryRequest schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceRepositoryDescriptionString\"\n        },\n        {\n          \"description\": \"The description of the source repository.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-create-source-repository-request-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: CreateSourceRepositoryRequest
---
