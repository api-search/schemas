---
description: Information about an upstream repository. A list of <code>UpstreamRepository</code> objects is an input parameter to <a href="https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_CreateRepository.html">CreateRepository</a> and <a href="https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_UpdateRepository.html">UpdateRepository</a>.
layout: schema
name: UpstreamRepository
properties_list:
- description: ''
  name: repositoryName
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-upstream-repository-schema.json
slug: codeartifact-upstream-repository
source_filename: codeartifact-upstream-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-upstream-repository-schema.json\",\n  \"title\": \"UpstreamRepository\",\n  \"description\": \" Information about an upstream repository. A list of <code>UpstreamRepository</code> objects is an input parameter to <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_CreateRepository.html\\\">CreateRepository</a> and <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_UpdateRepository.html\\\">UpdateRepository</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\": \" The name of an upstream repository. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"repositoryName\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-upstream-repository-schema.json
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
title: UpstreamRepository
---
