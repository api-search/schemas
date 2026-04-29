---
description: GetPackageVersionAssetResult schema from Amazon CodeArtifact API
layout: schema
name: GetPackageVersionAssetResult
properties_list:
- description: ''
  name: asset
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-get-package-version-asset-result-schema.json
slug: codeartifact-get-package-version-asset-result
source_filename: codeartifact-get-package-version-asset-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-get-package-version-asset-result-schema.json\",\n  \"title\": \"GetPackageVersionAssetResult\",\n  \"description\": \"GetPackageVersionAssetResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"asset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Asset\"\n        },\n        {\n          \"description\": \" The binary file, or asset, that is downloaded.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-get-package-version-asset-result-schema.json
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
title: GetPackageVersionAssetResult
---
