---
description: CreateRepositoryResult schema from Amazon CodeArtifact API
layout: schema
name: CreateRepositoryResult
properties_list:
- description: ''
  name: repository
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-create-repository-result-schema.json
slug: codeartifact-create-repository-result
source_filename: codeartifact-create-repository-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-create-repository-result-schema.json\",\n  \"title\": \"CreateRepositoryResult\",\n  \"description\": \"CreateRepositoryResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryDescription\"\n        },\n        {\n          \"description\": \" Information about the created repository after processing the request. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-create-repository-result-schema.json
tags:
- Amazon
- AWS
- Artifact Repository
- Package Management
- DevOps
- Software Supply Chain
- npm
- Maven
- PyPI
- NuGet
title: CreateRepositoryResult
---
