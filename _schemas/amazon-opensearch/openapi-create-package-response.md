---
description: Container for response returned by <code> <a>CreatePackage</a> </code> operation.
layout: schema
name: CreatePackageResponse
properties_list:
- description: ''
  name: PackageDetails
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-create-package-response-schema.json
slug: openapi-create-package-response
source_filename: openapi-create-package-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-package-response-schema.json\",\n  \"title\": \"CreatePackageResponse\",\n  \"description\": \" Container for response returned by <code> <a>CreatePackage</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PackageDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageDetails\"\n        },\n        {\n          \"description\": \"Information about the package <code>PackageDetails</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-create-package-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: CreatePackageResponse
---
