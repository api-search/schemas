---
description: DeletePackageResult schema from Amazon CodeArtifact API
layout: schema
name: DeletePackageResult
properties_list:
- description: ''
  name: deletedPackage
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-delete-package-result-schema.json
slug: codeartifact-delete-package-result
source_filename: codeartifact-delete-package-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-delete-package-result-schema.json\",\n  \"title\": \"DeletePackageResult\",\n  \"description\": \"DeletePackageResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deletedPackage\": {\n      \"$ref\": \"#/components/schemas/PackageSummary\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-delete-package-result-schema.json
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
title: DeletePackageResult
---
