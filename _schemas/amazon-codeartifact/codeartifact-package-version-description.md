---
description: Details about a package version.
layout: schema
name: PackageVersionDescription
properties_list:
- description: ''
  name: format
  type: object
- description: ''
  name: namespace
  type: object
- description: ''
  name: packageName
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: summary
  type: object
- description: ''
  name: homePage
  type: object
- description: ''
  name: sourceCodeRepository
  type: object
- description: ''
  name: publishedTime
  type: object
- description: ''
  name: licenses
  type: object
- description: ''
  name: revision
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: origin
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-package-version-description-schema.json
slug: codeartifact-package-version-description
source_filename: codeartifact-package-version-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-version-description-schema.json\",\n  \"title\": \"PackageVersionDescription\",\n  \"description\": \" Details about a package version. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageFormat\"\n        },\n        {\n          \"description\": \" The format of the package version. \"\n        }\n      ]\n    },\n    \"namespace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageNamespace\"\n        },\n        {\n          \"description\": \"<p>The namespace of the package version. The package version component that specifies its namespace depends on its type. For example:</p> <ul> <li> <p> The namespace of a Maven package version is its <code>groupId</code>.\
  \ </p> </li> <li> <p> The namespace of an npm package version is its <code>scope</code>. </p> </li> <li> <p> Python and NuGet package versions do not contain a corresponding component, package versions of those formats do not have a namespace. </p> </li> <li> <p> The namespace of a generic package is its <code>namespace</code>. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"packageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageName\"\n        },\n        {\n          \"description\": \" The name of the requested package. \"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String255\"\n        },\n        {\n          \"description\": \" The name of the package that is displayed. The <code>displayName</code> varies depending on the package version's format. For example, if an npm package is named <code>ui</code>, is in the namespace <code>vue</code>, and has\
  \ the format <code>npm</code>, then the <code>displayName</code> is <code>@vue/ui</code>. \"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersion\"\n        },\n        {\n          \"description\": \" The version of the package. \"\n        }\n      ]\n    },\n    \"summary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A summary of the package version. The summary is extracted from the package. The information in and detail level of the summary depends on the package version's format. \"\n        }\n      ]\n    },\n    \"homePage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The homepage associated with the package. \"\n        }\n      ]\n    },\n    \"sourceCodeRepository\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The repository for the source code in the package version, or the source code used to build it. \"\n        }\n      ]\n    },\n    \"publishedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" A timestamp that contains the date and time the package version was published. \"\n        }\n      ]\n    },\n    \"licenses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LicenseInfoList\"\n        },\n        {\n          \"description\": \" Information about licenses associated with the package version. \"\n        }\n      ]\n    },\n    \"revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionRevision\"\n        },\n        {\n          \"description\": \" The revision of the package version. \"\n        }\n\
  \      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionStatus\"\n        },\n        {\n          \"description\": \" A string that contains the status of the package version. \"\n        }\n      ]\n    },\n    \"origin\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionOrigin\"\n        },\n        {\n          \"description\": \"A <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionOrigin.html\\\">PackageVersionOrigin</a> object that contains information about how the package version was added to the repository.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-version-description-schema.json
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
title: PackageVersionDescription
---
