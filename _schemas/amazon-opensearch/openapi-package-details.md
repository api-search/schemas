---
description: Basic information about a package.
layout: schema
name: PackageDetails
properties_list:
- description: ''
  name: PackageID
  type: object
- description: ''
  name: PackageName
  type: object
- description: ''
  name: PackageType
  type: object
- description: ''
  name: PackageDescription
  type: object
- description: ''
  name: PackageStatus
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: LastUpdatedAt
  type: object
- description: ''
  name: AvailablePackageVersion
  type: object
- description: ''
  name: ErrorDetails
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-package-details-schema.json
slug: openapi-package-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-package-details-schema.json\",\n  \"title\": \"PackageDetails\",\n  \"description\": \"Basic information about a package.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PackageID\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageID\"\n        },\n        {\n          \"description\": \"Internal ID of the package.\"\n        }\n      ]\n    },\n    \"PackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageName\"\n        },\n        {\n          \"description\": \"User specified name of the package.\"\n        }\n      ]\n    },\n    \"PackageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageType\"\n        },\n        {\n          \"description\": \"Currently supports\
  \ only TXT-DICTIONARY.\"\n        }\n      ]\n    },\n    \"PackageDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageDescription\"\n        },\n        {\n          \"description\": \"User-specified description of the package.\"\n        }\n      ]\n    },\n    \"PackageStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageStatus\"\n        },\n        {\n          \"description\": \"Current state of the package. Values are COPYING/COPY_FAILED/AVAILABLE/DELETING/DELETE_FAILED\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"Timestamp which tells creation date of the package.\"\n        }\n      ]\n    },\n    \"LastUpdatedAt\": {\n      \"$ref\": \"#/components/schemas/LastUpdated\"\n    },\n    \"AvailablePackageVersion\": {\n      \"$ref\": \"#/components/schemas/PackageVersion\"\
  \n    },\n    \"ErrorDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorDetails\"\n        },\n        {\n          \"description\": \"Additional information if the package is in an error state. Null otherwise.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-package-details-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: PackageDetails
---
