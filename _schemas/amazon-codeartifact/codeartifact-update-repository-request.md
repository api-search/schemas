---
description: UpdateRepositoryRequest schema from Amazon CodeArtifact API
layout: schema
name: UpdateRepositoryRequest
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: upstreams
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-update-repository-request-schema.json
slug: codeartifact-update-repository-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-update-repository-request-schema.json\",\n  \"title\": \"UpdateRepositoryRequest\",\n  \"description\": \"UpdateRepositoryRequest schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \" An updated repository description. \"\n        }\n      ]\n    },\n    \"upstreams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpstreamRepositoryList\"\n        },\n        {\n          \"description\": \" A list of upstream repositories to associate with the repository. The order of the upstream repositories in the list determines their priority order when CodeArtifact looks\
  \ for a requested package version. For more information, see <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/ug/repos-upstream.html\\\">Working with upstream repositories</a>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-update-repository-request-schema.json
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
title: UpdateRepositoryRequest
---
