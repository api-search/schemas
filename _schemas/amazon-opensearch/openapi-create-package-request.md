---
description: Container for request parameters to <code> <a>CreatePackage</a> </code> operation.
layout: schema
name: CreatePackageRequest
properties_list:
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
  name: PackageSource
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-create-package-request-schema.json
slug: openapi-create-package-request
source_filename: openapi-create-package-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-package-request-schema.json\",\n  \"title\": \"CreatePackageRequest\",\n  \"description\": \" Container for request parameters to <code> <a>CreatePackage</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageName\"\n        },\n        {\n          \"description\": \"Unique identifier for the package.\"\n        }\n      ]\n    },\n    \"PackageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageType\"\n        },\n        {\n          \"description\": \"Type of package. Currently supports only TXT-DICTIONARY.\"\n        }\n      ]\n    },\n    \"PackageDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/PackageDescription\"\n        },\n        {\n          \"description\": \"Description of the package.\"\n        }\n      ]\n    },\n    \"PackageSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageSource\"\n        },\n        {\n          \"description\": \"The customer S3 location <code>PackageSource</code> for importing the package.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PackageName\",\n    \"PackageType\",\n    \"PackageSource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-package-request-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: CreatePackageRequest
---
