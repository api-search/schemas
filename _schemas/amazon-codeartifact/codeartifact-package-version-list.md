---
description: PackageVersionList schema from Amazon CodeArtifact API
layout: schema
name: PackageVersionList
properties_list: []
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-package-version-list-schema.json
slug: codeartifact-package-version-list
source_filename: codeartifact-package-version-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-version-list-schema.json\",\n  \"title\": \"PackageVersionList\",\n  \"description\": \"PackageVersionList schema from Amazon CodeArtifact API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/PackageVersion\"\n  },\n  \"maxItems\": 100\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-version-list-schema.json
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
title: PackageVersionList
---
