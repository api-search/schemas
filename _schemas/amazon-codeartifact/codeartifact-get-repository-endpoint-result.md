---
description: GetRepositoryEndpointResult schema from Amazon CodeArtifact API
layout: schema
name: GetRepositoryEndpointResult
properties_list:
- description: ''
  name: repositoryEndpoint
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-get-repository-endpoint-result-schema.json
slug: codeartifact-get-repository-endpoint-result
source_filename: codeartifact-get-repository-endpoint-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-get-repository-endpoint-result-schema.json\",\n  \"title\": \"GetRepositoryEndpointResult\",\n  \"description\": \"GetRepositoryEndpointResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repositoryEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A string that specifies the URL of the returned endpoint. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-get-repository-endpoint-result-schema.json
tags:
- Amazon
- Artifact Repository
- Package Management
- DevOps
- Software Supply Chain
- npm
- Maven
- PyPI
- NuGet
title: GetRepositoryEndpointResult
---
