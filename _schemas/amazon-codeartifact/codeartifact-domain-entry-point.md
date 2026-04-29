---
description: Information about how a package originally entered the CodeArtifact domain. For packages published directly to CodeArtifact, the entry point is the repository it was published to. For packages ingested from an external repository, the entry point is the external connection that it was ingested from. An external connection is a CodeArtifact repository that is connected to an external repository such as the npm registry or NuGet gallery.
layout: schema
name: DomainEntryPoint
properties_list:
- description: ''
  name: repositoryName
  type: object
- description: ''
  name: externalConnectionName
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-domain-entry-point-schema.json
slug: codeartifact-domain-entry-point
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-domain-entry-point-schema.json\",\n  \"title\": \"DomainEntryPoint\",\n  \"description\": \"Information about how a package originally entered the CodeArtifact domain. For packages published directly to CodeArtifact, the entry point is the repository it was published to. For packages ingested from an external repository, the entry point is the external connection that it was ingested from. An external connection is a CodeArtifact repository that is connected to an external repository such as the npm registry or NuGet gallery.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\": \"The name of the repository that a package was\
  \ originally published to.\"\n        }\n      ]\n    },\n    \"externalConnectionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalConnectionName\"\n        },\n        {\n          \"description\": \"The name of the external connection that a package was ingested from.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-domain-entry-point-schema.json
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
title: DomainEntryPoint
---
