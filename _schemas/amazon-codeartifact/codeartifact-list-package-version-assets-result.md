---
description: ListPackageVersionAssetsResult schema from Amazon CodeArtifact API
layout: schema
name: ListPackageVersionAssetsResult
properties_list:
- description: ''
  name: format
  type: object
- description: ''
  name: namespace
  type: object
- description: ''
  name: package
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: versionRevision
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: assets
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-list-package-version-assets-result-schema.json
slug: codeartifact-list-package-version-assets-result
source_filename: codeartifact-list-package-version-assets-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-list-package-version-assets-result-schema.json\",\n  \"title\": \"ListPackageVersionAssetsResult\",\n  \"description\": \"ListPackageVersionAssetsResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageFormat\"\n        },\n        {\n          \"description\": \" The format of the package that contains the requested package version assets. \"\n        }\n      ]\n    },\n    \"namespace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageNamespace\"\n        },\n        {\n          \"description\": \"<p>The namespace of the package version that contains the requested package version assets. The package version component\
  \ that specifies its namespace depends on its type. For example:</p> <ul> <li> <p> The namespace of a Maven package version is its <code>groupId</code>. </p> </li> <li> <p> The namespace of an npm package version is its <code>scope</code>. </p> </li> <li> <p> Python and NuGet package versions do not contain a corresponding component, package versions of those formats do not have a namespace. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"package\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageName\"\n        },\n        {\n          \"description\": \" The name of the package that contains the requested package version assets. \"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersion\"\n        },\n        {\n          \"description\": \" The version of the package associated with the requested assets. \"\n        }\n      ]\n    },\n    \"versionRevision\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionRevision\"\n        },\n        {\n          \"description\": \" The current revision associated with the package version. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \" If there are additional results, this is the token for the next set of results. \"\n        }\n      ]\n    },\n    \"assets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetSummaryList\"\n        },\n        {\n          \"description\": \" The returned list of <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_AssetSummary.html\\\">AssetSummary</a> objects. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-list-package-version-assets-result-schema.json
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
title: ListPackageVersionAssetsResult
---
