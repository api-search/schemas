---
description: Information about an upstream repository.
layout: schema
name: UpstreamRepositoryInfo
properties_list:
- description: ''
  name: repositoryName
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-upstream-repository-info-schema.json
slug: codeartifact-upstream-repository-info
source_filename: codeartifact-upstream-repository-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-upstream-repository-info-schema.json\",\n  \"title\": \"UpstreamRepositoryInfo\",\n  \"description\": \" Information about an upstream repository. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\": \" The name of an upstream repository. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-upstream-repository-info-schema.json
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
title: UpstreamRepositoryInfo
---
