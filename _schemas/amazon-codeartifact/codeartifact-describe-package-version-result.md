---
description: DescribePackageVersionResult schema from Amazon CodeArtifact API
layout: schema
name: DescribePackageVersionResult
properties_list:
- description: ''
  name: packageVersion
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-describe-package-version-result-schema.json
slug: codeartifact-describe-package-version-result
source_filename: codeartifact-describe-package-version-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-describe-package-version-result-schema.json\",\n  \"title\": \"DescribePackageVersionResult\",\n  \"description\": \"DescribePackageVersionResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"packageVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionDescription\"\n        },\n        {\n          \"description\": \" A <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionDescription.html\\\">PackageVersionDescription</a> object that contains information about the requested package version. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"packageVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-describe-package-version-result-schema.json
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
title: DescribePackageVersionResult
---
