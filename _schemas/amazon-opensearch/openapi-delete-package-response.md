---
description: Container for response parameters to <code> <a>DeletePackage</a> </code> operation.
layout: schema
name: DeletePackageResponse
properties_list:
- description: ''
  name: PackageDetails
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-delete-package-response-schema.json
slug: openapi-delete-package-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-delete-package-response-schema.json\",\n  \"title\": \"DeletePackageResponse\",\n  \"description\": \" Container for response parameters to <code> <a>DeletePackage</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PackageDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageDetails\"\n        },\n        {\n          \"description\": \"<code>PackageDetails</code>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-delete-package-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DeletePackageResponse
---
