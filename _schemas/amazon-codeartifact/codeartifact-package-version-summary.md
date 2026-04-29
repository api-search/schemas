---
description: Details about a package version, including its status, version, and revision. The <a href="https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_ListPackageVersions.html">ListPackageVersions</a> operation returns a list of <code>PackageVersionSummary</code> objects.
layout: schema
name: PackageVersionSummary
properties_list:
- description: ''
  name: version
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
schema_file: json-schema/codeartifact-package-version-summary-schema.json
slug: codeartifact-package-version-summary
source_filename: codeartifact-package-version-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-version-summary-schema.json\",\n  \"title\": \"PackageVersionSummary\",\n  \"description\": \" Details about a package version, including its status, version, and revision. The <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_ListPackageVersions.html\\\">ListPackageVersions</a> operation returns a list of <code>PackageVersionSummary</code> objects. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersion\"\n        },\n        {\n          \"description\": \" Information about a package version. \"\n        }\n      ]\n    },\n    \"revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionRevision\"\n  \
  \      },\n        {\n          \"description\": \" The revision associated with a package version. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionStatus\"\n        },\n        {\n          \"description\": \" A string that contains the status of the package version. It can be one of the following: \"\n        }\n      ]\n    },\n    \"origin\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionOrigin\"\n        },\n        {\n          \"description\": \"A <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageVersionOrigin.html\\\">PackageVersionOrigin</a> object that contains information about how the package version was added to the repository.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"version\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-version-summary-schema.json
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
title: PackageVersionSummary
---
