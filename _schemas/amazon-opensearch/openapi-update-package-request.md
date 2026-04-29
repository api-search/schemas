---
description: Container for request parameters to <code> <a>UpdatePackage</a> </code> operation.
layout: schema
name: UpdatePackageRequest
properties_list:
- description: ''
  name: PackageID
  type: object
- description: ''
  name: PackageSource
  type: object
- description: ''
  name: PackageDescription
  type: object
- description: ''
  name: CommitMessage
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-update-package-request-schema.json
slug: openapi-update-package-request
source_filename: openapi-update-package-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-update-package-request-schema.json\",\n  \"title\": \"UpdatePackageRequest\",\n  \"description\": \" Container for request parameters to <code> <a>UpdatePackage</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PackageID\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageID\"\n        },\n        {\n          \"description\": \"Unique identifier for the package.\"\n        }\n      ]\n    },\n    \"PackageSource\": {\n      \"$ref\": \"#/components/schemas/PackageSource\"\n    },\n    \"PackageDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageDescription\"\n        },\n        {\n          \"description\": \"New description of the package.\"\n        }\n      ]\n    },\n    \"CommitMessage\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CommitMessage\"\n        },\n        {\n          \"description\": \"An info message for the new version which will be shown as part of <code>GetPackageVersionHistoryResponse</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PackageID\",\n    \"PackageSource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-update-package-request-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: UpdatePackageRequest
---
