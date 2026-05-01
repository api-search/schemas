---
description: l An error associated with package.
layout: schema
name: PackageVersionError
properties_list:
- description: ''
  name: errorCode
  type: object
- description: ''
  name: errorMessage
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-package-version-error-schema.json
slug: codeartifact-package-version-error
source_filename: codeartifact-package-version-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-version-error-schema.json\",\n  \"title\": \"PackageVersionError\",\n  \"description\": \"l An error associated with package. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionErrorCode\"\n        },\n        {\n          \"description\": \"<p> The error code associated with the error. Valid error codes are: </p> <ul> <li> <p> <code>ALREADY_EXISTS</code> </p> </li> <li> <p> <code>MISMATCHED_REVISION</code> </p> </li> <li> <p> <code>MISMATCHED_STATUS</code> </p> </li> <li> <p> <code>NOT_ALLOWED</code> </p> </li> <li> <p> <code>NOT_FOUND</code> </p> </li> <li> <p> <code>SKIPPED</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ErrorMessage\"\n        },\n        {\n          \"description\": \" The error message associated with the error. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-version-error-schema.json
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
title: PackageVersionError
---
