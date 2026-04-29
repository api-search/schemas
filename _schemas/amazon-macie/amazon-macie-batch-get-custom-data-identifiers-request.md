---
description: BatchGetCustomDataIdentifiersRequest schema from Amazon Macie API
layout: schema
name: BatchGetCustomDataIdentifiersRequest
properties_list:
- description: ''
  name: ids
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-batch-get-custom-data-identifiers-request-schema.json
slug: amazon-macie-batch-get-custom-data-identifiers-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-batch-get-custom-data-identifiers-request-schema.json\",\n  \"title\": \"BatchGetCustomDataIdentifiersRequest\",\n  \"description\": \"BatchGetCustomDataIdentifiersRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array of custom data identifier IDs, one for each custom data identifier to retrieve information about.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-batch-get-custom-data-identifiers-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BatchGetCustomDataIdentifiersRequest
---
