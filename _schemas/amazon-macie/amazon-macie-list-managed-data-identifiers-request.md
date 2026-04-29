---
description: ListManagedDataIdentifiersRequest schema from Amazon Macie API
layout: schema
name: ListManagedDataIdentifiersRequest
properties_list:
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-list-managed-data-identifiers-request-schema.json
slug: amazon-macie-list-managed-data-identifiers-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-managed-data-identifiers-request-schema.json\",\n  \"title\": \"ListManagedDataIdentifiersRequest\",\n  \"description\": \"ListManagedDataIdentifiersRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The nextToken string that specifies which page of results to return in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-managed-data-identifiers-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ListManagedDataIdentifiersRequest
---
