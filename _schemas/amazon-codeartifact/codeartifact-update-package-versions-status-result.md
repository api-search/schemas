---
description: UpdatePackageVersionsStatusResult schema from Amazon CodeArtifact API
layout: schema
name: UpdatePackageVersionsStatusResult
properties_list:
- description: ''
  name: successfulVersions
  type: object
- description: ''
  name: failedVersions
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-update-package-versions-status-result-schema.json
slug: codeartifact-update-package-versions-status-result
source_filename: codeartifact-update-package-versions-status-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-update-package-versions-status-result-schema.json\",\n  \"title\": \"UpdatePackageVersionsStatusResult\",\n  \"description\": \"UpdatePackageVersionsStatusResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"successfulVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SuccessfulPackageVersionInfoMap\"\n        },\n        {\n          \"description\": \" A list of <code>PackageVersionError</code> objects, one for each package version with a status that failed to update. \"\n        }\n      ]\n    },\n    \"failedVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionErrorMap\"\n        },\n        {\n          \"description\": \" A list of <code>SuccessfulPackageVersionInfo</code>\
  \ objects, one for each package version with a status that successfully updated. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-update-package-versions-status-result-schema.json
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
title: UpdatePackageVersionsStatusResult
---
