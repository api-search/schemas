---
description: Information about how a package version was added to a repository.
layout: schema
name: PackageVersionOrigin
properties_list:
- description: ''
  name: domainEntryPoint
  type: object
- description: ''
  name: originType
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-package-version-origin-schema.json
slug: codeartifact-package-version-origin
source_filename: codeartifact-package-version-origin-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-version-origin-schema.json\",\n  \"title\": \"PackageVersionOrigin\",\n  \"description\": \"Information about how a package version was added to a repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainEntryPoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainEntryPoint\"\n        },\n        {\n          \"description\": \"A <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_DomainEntryPoint.html\\\">DomainEntryPoint</a> object that contains information about from which repository or external connection the package version was added to the domain.\"\n        }\n      ]\n    },\n    \"originType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionOriginType\"\
  \n        },\n        {\n          \"description\": \"Describes how the package version was originally added to the domain. An <code>INTERNAL</code> origin type means the package version was published directly to a repository in the domain. An <code>EXTERNAL</code> origin type means the package version was ingested from an external connection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-version-origin-schema.json
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
title: PackageVersionOrigin
---
