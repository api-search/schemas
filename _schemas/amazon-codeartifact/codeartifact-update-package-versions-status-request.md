---
description: UpdatePackageVersionsStatusRequest schema from Amazon CodeArtifact API
layout: schema
name: UpdatePackageVersionsStatusRequest
properties_list:
- description: ''
  name: versions
  type: object
- description: ''
  name: versionRevisions
  type: object
- description: ''
  name: expectedStatus
  type: object
- description: ''
  name: targetStatus
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-update-package-versions-status-request-schema.json
slug: codeartifact-update-package-versions-status-request
source_filename: codeartifact-update-package-versions-status-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-update-package-versions-status-request-schema.json\",\n  \"title\": \"UpdatePackageVersionsStatusRequest\",\n  \"description\": \"UpdatePackageVersionsStatusRequest schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"versions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionList\"\n        },\n        {\n          \"description\": \" An array of strings that specify the versions of the package with the statuses to update. \"\n        }\n      ]\n    },\n    \"versionRevisions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionRevisionMap\"\n        },\n        {\n          \"description\": \" A map of package versions and package version revisions. The map <code>key</code>\
  \ is the package version (for example, <code>3.5.2</code>), and the map <code>value</code> is the package version revision. \"\n        }\n      ]\n    },\n    \"expectedStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionStatus\"\n        },\n        {\n          \"description\": \" The package version\\u2019s expected status before it is updated. If <code>expectedStatus</code> is provided, the package version's status is updated only if its status at the time <code>UpdatePackageVersionsStatus</code> is called matches <code>expectedStatus</code>. \"\n        }\n      ]\n    },\n    \"targetStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionStatus\"\n        },\n        {\n          \"description\": \" The status you want to change the package version status to. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"versions\",\n    \"targetStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-update-package-versions-status-request-schema.json
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
title: UpdatePackageVersionsStatusRequest
---
