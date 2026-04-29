---
description: DisposePackageVersionsRequest schema from Amazon CodeArtifact API
layout: schema
name: DisposePackageVersionsRequest
properties_list:
- description: ''
  name: versions
  type: object
- description: ''
  name: versionRevisions
  type: object
- description: ''
  name: expectedStatus
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-dispose-package-versions-request-schema.json
slug: codeartifact-dispose-package-versions-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-dispose-package-versions-request-schema.json\",\n  \"title\": \"DisposePackageVersionsRequest\",\n  \"description\": \"DisposePackageVersionsRequest schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"versions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionList\"\n        },\n        {\n          \"description\": \" The versions of the package you want to dispose. \"\n        }\n      ]\n    },\n    \"versionRevisions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionRevisionMap\"\n        },\n        {\n          \"description\": \" The revisions of the package versions you want to dispose. \"\n        }\n      ]\n    },\n    \"expectedStatus\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionStatus\"\n        },\n        {\n          \"description\": \" The expected status of the package version to dispose. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"versions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-dispose-package-versions-request-schema.json
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
title: DisposePackageVersionsRequest
---
