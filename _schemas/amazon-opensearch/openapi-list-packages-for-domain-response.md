---
description: Container for response parameters to <code> <a>ListPackagesForDomain</a> </code> operation.
layout: schema
name: ListPackagesForDomainResponse
properties_list:
- description: ''
  name: DomainPackageDetailsList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-list-packages-for-domain-response-schema.json
slug: openapi-list-packages-for-domain-response
source_filename: openapi-list-packages-for-domain-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-packages-for-domain-response-schema.json\",\n  \"title\": \"ListPackagesForDomainResponse\",\n  \"description\": \" Container for response parameters to <code> <a>ListPackagesForDomain</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainPackageDetailsList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainPackageDetailsList\"\n        },\n        {\n          \"description\": \"List of <code>DomainPackageDetails</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Pagination token that needs to be supplied to the next call to get the next page of results.\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-packages-for-domain-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: ListPackagesForDomainResponse
---
