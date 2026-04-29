---
description: Details about a package dependency.
layout: schema
name: PackageDependency
properties_list:
- description: ''
  name: namespace
  type: object
- description: ''
  name: package
  type: object
- description: ''
  name: dependencyType
  type: object
- description: ''
  name: versionRequirement
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-package-dependency-schema.json
slug: codeartifact-package-dependency
source_filename: codeartifact-package-dependency-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-dependency-schema.json\",\n  \"title\": \"PackageDependency\",\n  \"description\": \" Details about a package dependency. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageNamespace\"\n        },\n        {\n          \"description\": \"<p>The namespace of the package that this package depends on. The package component that specifies its namespace depends on its type. For example:</p> <ul> <li> <p> The namespace of a Maven package is its <code>groupId</code>. </p> </li> <li> <p> The namespace of an npm package is its <code>scope</code>. </p> </li> <li> <p> Python and NuGet packages do not contain a corresponding component, packages of those formats do not have a namespace. </p>\
  \ </li> </ul>\"\n        }\n      ]\n    },\n    \"package\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageName\"\n        },\n        {\n          \"description\": \" The name of the package that this package depends on. \"\n        }\n      ]\n    },\n    \"dependencyType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p> The type of a package dependency. The possible values depend on the package type.</p> <ul> <li> <p>npm: <code>regular</code>, <code>dev</code>, <code>peer</code>, <code>optional</code> </p> </li> <li> <p>maven: <code>optional</code>, <code>parent</code>, <code>compile</code>, <code>runtime</code>, <code>test</code>, <code>system</code>, <code>provided</code>.</p> <note> <p>Note that <code>parent</code> is not a regular Maven dependency type; instead this is extracted from the <code>&lt;parent&gt;</code> element if one is defined in the\
  \ package version's POM file.</p> </note> </li> <li> <p>nuget: The <code>dependencyType</code> field is never set for NuGet packages.</p> </li> <li> <p>pypi: <code>Requires-Dist</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"versionRequirement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The required version, or version range, of the package that this package depends on. The version format is specific to the package type. For example, the following are possible valid required versions: <code>1.2.3</code>, <code>^2.3.4</code>, or <code>4.x</code>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-dependency-schema.json
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
title: PackageDependency
---
