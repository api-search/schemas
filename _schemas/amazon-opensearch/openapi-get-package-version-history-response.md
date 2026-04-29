---
description: Container for response returned by <code> <a>GetPackageVersionHistory</a> </code> operation.
layout: schema
name: GetPackageVersionHistoryResponse
properties_list:
- description: ''
  name: PackageID
  type: object
- description: ''
  name: PackageVersionHistoryList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-get-package-version-history-response-schema.json
slug: openapi-get-package-version-history-response
source_filename: openapi-get-package-version-history-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-get-package-version-history-response-schema.json\",\n  \"title\": \"GetPackageVersionHistoryResponse\",\n  \"description\": \" Container for response returned by <code> <a>GetPackageVersionHistory</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PackageID\": {\n      \"$ref\": \"#/components/schemas/PackageID\"\n    },\n    \"PackageVersionHistoryList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageVersionHistoryList\"\n        },\n        {\n          \"description\": \"List of <code>PackageVersionHistory</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/String\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-get-package-version-history-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: GetPackageVersionHistoryResponse
---
