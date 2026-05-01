---
description: PublishPackageVersionResult schema from Amazon CodeArtifact API
layout: schema
name: PublishPackageVersionResult
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
  name: status
  type: object
- description: ''
  name: asset
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-publish-package-version-result-schema.json
slug: codeartifact-publish-package-version-result
source_filename: codeartifact-publish-package-version-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-publish-package-version-result-schema.json\",\n  \"title\": \"PublishPackageVersionResult\",\n  \"description\": \"PublishPackageVersionResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageFormat\"\n        },\n        {\n          \"description\": \"The format of the package version.\"\n        }\n      ]\n    },\n    \"namespace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageNamespace\"\n        },\n        {\n          \"description\": \"The namespace of the package version.\"\n        }\n      ]\n    },\n    \"package\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageName\"\
  \n        },\n        {\n          \"description\": \"The name of the package.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersion\"\n        },\n        {\n          \"description\": \"The version of the package.\"\n        }\n      ]\n    },\n    \"versionRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionRevision\"\n        },\n        {\n          \"description\": \"The revision of the package version.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionStatus\"\n        },\n        {\n          \"description\": \"A string that contains the status of the package version. For more information, see <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/ug/packages-overview.html#package-version-status.html#package-version-status\\\">Package version status</a>\
  \ in the <i>CodeArtifact User Guide</i>.\"\n        }\n      ]\n    },\n    \"asset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssetSummary\"\n        },\n        {\n          \"description\": \"An <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_AssetSummary.html\\\">AssetSummary</a> for the published asset.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-publish-package-version-result-schema.json
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
title: PublishPackageVersionResult
---
