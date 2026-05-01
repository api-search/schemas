---
description: ErrorDetails schema from Amazon OpenSearch Service API
layout: schema
name: ErrorDetails
properties_list:
- description: ''
  name: ErrorType
  type: object
- description: ''
  name: ErrorMessage
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-error-details-schema.json
slug: openapi-error-details
source_filename: openapi-error-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-error-details-schema.json\",\n  \"title\": \"ErrorDetails\",\n  \"description\": \"ErrorDetails schema from Amazon OpenSearch Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ErrorType\": {\n      \"$ref\": \"#/components/schemas/ErrorType\"\n    },\n    \"ErrorMessage\": {\n      \"$ref\": \"#/components/schemas/ErrorMessage\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-error-details-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: ErrorDetails
---
