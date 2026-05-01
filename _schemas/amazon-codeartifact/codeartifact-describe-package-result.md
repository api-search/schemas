---
description: DescribePackageResult schema from Amazon CodeArtifact API
layout: schema
name: DescribePackageResult
properties_list:
- description: ''
  name: package
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-describe-package-result-schema.json
slug: codeartifact-describe-package-result
source_filename: codeartifact-describe-package-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-describe-package-result-schema.json\",\n  \"title\": \"DescribePackageResult\",\n  \"description\": \"DescribePackageResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"package\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageDescription\"\n        },\n        {\n          \"description\": \"A <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageDescription.html\\\">PackageDescription</a> object that contains information about the requested package.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"package\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-describe-package-result-schema.json
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
title: DescribePackageResult
---
