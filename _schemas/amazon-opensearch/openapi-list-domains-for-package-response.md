---
description: Container for response parameters to <code> <a>ListDomainsForPackage</a> </code> operation.
layout: schema
name: ListDomainsForPackageResponse
properties_list:
- description: ''
  name: DomainPackageDetailsList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-list-domains-for-package-response-schema.json
slug: openapi-list-domains-for-package-response
source_filename: openapi-list-domains-for-package-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-domains-for-package-response-schema.json\",\n  \"title\": \"ListDomainsForPackageResponse\",\n  \"description\": \" Container for response parameters to <code> <a>ListDomainsForPackage</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainPackageDetailsList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainPackageDetailsList\"\n        },\n        {\n          \"description\": \"List of <code>DomainPackageDetails</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/String\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-domains-for-package-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: ListDomainsForPackageResponse
---
