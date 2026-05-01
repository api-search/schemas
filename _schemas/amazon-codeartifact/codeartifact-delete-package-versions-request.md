---
description: DeletePackageVersionsRequest schema from Amazon CodeArtifact API
layout: schema
name: DeletePackageVersionsRequest
properties_list:
- description: ''
  name: versions
  type: object
- description: ''
  name: expectedStatus
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-delete-package-versions-request-schema.json
slug: codeartifact-delete-package-versions-request
source_filename: codeartifact-delete-package-versions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-delete-package-versions-request-schema.json\",\n  \"title\": \"DeletePackageVersionsRequest\",\n  \"description\": \"DeletePackageVersionsRequest schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"versions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionList\"\n        },\n        {\n          \"description\": \" An array of strings that specify the versions of the package to delete. \"\n        }\n      ]\n    },\n    \"expectedStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionStatus\"\n        },\n        {\n          \"description\": \" The expected status of the package version to delete. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n \
  \   \"versions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-delete-package-versions-request-schema.json
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
title: DeletePackageVersionsRequest
---
