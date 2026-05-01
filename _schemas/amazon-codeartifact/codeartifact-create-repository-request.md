---
description: CreateRepositoryRequest schema from Amazon CodeArtifact API
layout: schema
name: CreateRepositoryRequest
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: upstreams
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-create-repository-request-schema.json
slug: codeartifact-create-repository-request
source_filename: codeartifact-create-repository-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-create-repository-request-schema.json\",\n  \"title\": \"CreateRepositoryRequest\",\n  \"description\": \"CreateRepositoryRequest schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \" A description of the created repository. \"\n        }\n      ]\n    },\n    \"upstreams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpstreamRepositoryList\"\n        },\n        {\n          \"description\": \" A list of upstream repositories to associate with the repository. The order of the upstream repositories in the list determines their priority order when CodeArtifact\
  \ looks for a requested package version. For more information, see <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/ug/repos-upstream.html\\\">Working with upstream repositories</a>. \"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"One or more tag key-value pairs for the repository.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-create-repository-request-schema.json
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
title: CreateRepositoryRequest
---
