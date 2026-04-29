---
description: Contains the revision and status of a package version.
layout: schema
name: SuccessfulPackageVersionInfo
properties_list:
- description: ''
  name: revision
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-successful-package-version-info-schema.json
slug: codeartifact-successful-package-version-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-successful-package-version-info-schema.json\",\n  \"title\": \"SuccessfulPackageVersionInfo\",\n  \"description\": \" Contains the revision and status of a package version. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The revision of a package version. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionStatus\"\n        },\n        {\n          \"description\": \" The status of a package version. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-successful-package-version-info-schema.json
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
title: SuccessfulPackageVersionInfo
---
