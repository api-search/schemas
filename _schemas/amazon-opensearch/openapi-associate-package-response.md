---
description: Container for response returned by <code> <a>AssociatePackage</a> </code> operation.
layout: schema
name: AssociatePackageResponse
properties_list:
- description: ''
  name: DomainPackageDetails
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-associate-package-response-schema.json
slug: openapi-associate-package-response
source_filename: openapi-associate-package-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-associate-package-response-schema.json\",\n  \"title\": \"AssociatePackageResponse\",\n  \"description\": \" Container for response returned by <code> <a>AssociatePackage</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainPackageDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainPackageDetails\"\n        },\n        {\n          \"description\": \"<code>DomainPackageDetails</code>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-associate-package-response-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: AssociatePackageResponse
---
