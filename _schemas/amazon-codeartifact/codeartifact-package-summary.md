---
description: Details about a package, including its format, namespace, and name.
layout: schema
name: PackageSummary
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
  name: originConfiguration
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-package-summary-schema.json
slug: codeartifact-package-summary
source_filename: codeartifact-package-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-summary-schema.json\",\n  \"title\": \"PackageSummary\",\n  \"description\": \" Details about a package, including its format, namespace, and name. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageFormat\"\n        },\n        {\n          \"description\": \" The format of the package. \"\n        }\n      ]\n    },\n    \"namespace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageNamespace\"\n        },\n        {\n          \"description\": \"<p>The namespace of the package. The package component that specifies its namespace depends on its type. For example:</p> <ul> <li> <p> The namespace of a Maven package is its <code>groupId</code>. </p>\
  \ </li> <li> <p> The namespace of an npm package is its <code>scope</code>. </p> </li> <li> <p> Python and NuGet packages do not contain a corresponding component, packages of those formats do not have a namespace. </p> </li> <li> <p> The namespace of a generic package is its <code>namespace</code>. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"package\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageName\"\n        },\n        {\n          \"description\": \" The name of the package. \"\n        }\n      ]\n    },\n    \"originConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageOriginConfiguration\"\n        },\n        {\n          \"description\": \"A <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageOriginConfiguration.html\\\">PackageOriginConfiguration</a> object that contains a <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageOriginRestrictions.html\\\
  \">PackageOriginRestrictions</a> object that contains information about the upstream and publish package origin restrictions.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-summary-schema.json
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
title: PackageSummary
---
