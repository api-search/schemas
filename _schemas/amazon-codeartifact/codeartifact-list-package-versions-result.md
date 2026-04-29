---
description: ListPackageVersionsResult schema from Amazon CodeArtifact API
layout: schema
name: ListPackageVersionsResult
properties_list:
- description: ''
  name: defaultDisplayVersion
  type: object
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
  name: versions
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-list-package-versions-result-schema.json
slug: codeartifact-list-package-versions-result
source_filename: codeartifact-list-package-versions-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-list-package-versions-result-schema.json\",\n  \"title\": \"ListPackageVersionsResult\",\n  \"description\": \"ListPackageVersionsResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"defaultDisplayVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersion\"\n        },\n        {\n          \"description\": \"<p> The default package version to display. This depends on the package format: </p> <ul> <li> <p> For Maven and PyPI packages, it's the most recently published package version. </p> </li> <li> <p> For npm packages, it's the version referenced by the <code>latest</code> tag. If the <code>latest</code> tag is not set, it's the most recently published package version. </p> </li> </ul>\"\n     \
  \   }\n      ]\n    },\n    \"format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageFormat\"\n        },\n        {\n          \"description\": \" A format of the package. \"\n        }\n      ]\n    },\n    \"namespace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageNamespace\"\n        },\n        {\n          \"description\": \"<p>The namespace of the package that contains the requested package versions. The package component that specifies its namespace depends on its type. For example:</p> <ul> <li> <p> The namespace of a Maven package is its <code>groupId</code>. </p> </li> <li> <p> The namespace of an npm package is its <code>scope</code>. </p> </li> <li> <p> Python and NuGet packages do not contain a corresponding component, packages of those formats do not have a namespace. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"package\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageName\"\
  \n        },\n        {\n          \"description\": \" The name of the package. \"\n        }\n      ]\n    },\n    \"versions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionSummaryList\"\n        },\n        {\n          \"description\": \" The returned list of <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionSummary.html\\\">PackageVersionSummary</a> objects. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \" If there are additional results, this is the token for the next set of results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-list-package-versions-result-schema.json
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
title: ListPackageVersionsResult
---
