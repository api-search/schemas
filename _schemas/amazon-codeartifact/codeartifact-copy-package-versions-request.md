---
description: CopyPackageVersionsRequest schema from Amazon CodeArtifact API
layout: schema
name: CopyPackageVersionsRequest
properties_list:
- description: ''
  name: versions
  type: object
- description: ''
  name: versionRevisions
  type: object
- description: ''
  name: allowOverwrite
  type: object
- description: ''
  name: includeFromUpstream
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-copy-package-versions-request-schema.json
slug: codeartifact-copy-package-versions-request
source_filename: codeartifact-copy-package-versions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-copy-package-versions-request-schema.json\",\n  \"title\": \"CopyPackageVersionsRequest\",\n  \"description\": \"CopyPackageVersionsRequest schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"versions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionList\"\n        },\n        {\n          \"description\": \"<p> The versions of the package to be copied. </p> <note> <p> You must specify <code>versions</code> or <code>versionRevisions</code>. You cannot specify both. </p> </note>\"\n        }\n      ]\n    },\n    \"versionRevisions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionRevisionMap\"\n        },\n        {\n          \"description\": \"<p> A list of\
  \ key-value pairs. The keys are package versions and the values are package version revisions. A <code>CopyPackageVersion</code> operation succeeds if the specified versions in the source repository match the specified package version revision. </p> <note> <p> You must specify <code>versions</code> or <code>versionRevisions</code>. You cannot specify both. </p> </note>\"\n        }\n      ]\n    },\n    \"allowOverwrite\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanOptional\"\n        },\n        {\n          \"description\": \" Set to true to overwrite a package version that already exists in the destination repository. If set to false and the package version already exists in the destination repository, the package version is returned in the <code>failedVersions</code> field of the response with an <code>ALREADY_EXISTS</code> error code. \"\n        }\n      ]\n    },\n    \"includeFromUpstream\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/BooleanOptional\"\n        },\n        {\n          \"description\": \" Set to true to copy packages from repositories that are upstream from the source repository to the destination repository. The default setting is false. For more information, see <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/ug/repos-upstream.html\\\">Working with upstream repositories</a>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-copy-package-versions-request-schema.json
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
title: CopyPackageVersionsRequest
---
