---
description: DeletePackageVersionsResult schema from Amazon CodeArtifact API
layout: schema
name: DeletePackageVersionsResult
properties_list:
- description: ''
  name: successfulVersions
  type: object
- description: ''
  name: failedVersions
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-delete-package-versions-result-schema.json
slug: codeartifact-delete-package-versions-result
source_filename: codeartifact-delete-package-versions-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-delete-package-versions-result-schema.json\",\n  \"title\": \"DeletePackageVersionsResult\",\n  \"description\": \"DeletePackageVersionsResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"successfulVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SuccessfulPackageVersionInfoMap\"\n        },\n        {\n          \"description\": \" A list of the package versions that were successfully deleted. The status of every successful version will be <code>Deleted</code>. \"\n        }\n      ]\n    },\n    \"failedVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionErrorMap\"\n        },\n        {\n          \"description\": \"<p> A <code>PackageVersionError</code>\
  \ object that contains a map of errors codes for the deleted package that failed. The possible error codes are: </p> <ul> <li> <p> <code>ALREADY_EXISTS</code> </p> </li> <li> <p> <code>MISMATCHED_REVISION</code> </p> </li> <li> <p> <code>MISMATCHED_STATUS</code> </p> </li> <li> <p> <code>NOT_ALLOWED</code> </p> </li> <li> <p> <code>NOT_FOUND</code> </p> </li> <li> <p> <code>SKIPPED</code> </p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-delete-package-versions-result-schema.json
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
title: DeletePackageVersionsResult
---
