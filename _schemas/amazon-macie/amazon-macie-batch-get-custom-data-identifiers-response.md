---
description: BatchGetCustomDataIdentifiersResponse schema from Amazon Macie API
layout: schema
name: BatchGetCustomDataIdentifiersResponse
properties_list:
- description: ''
  name: customDataIdentifiers
  type: object
- description: ''
  name: notFoundIdentifierIds
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-batch-get-custom-data-identifiers-response-schema.json
slug: amazon-macie-batch-get-custom-data-identifiers-response
source_filename: amazon-macie-batch-get-custom-data-identifiers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-batch-get-custom-data-identifiers-response-schema.json\",\n  \"title\": \"BatchGetCustomDataIdentifiersResponse\",\n  \"description\": \"BatchGetCustomDataIdentifiersResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customDataIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfBatchGetCustomDataIdentifierSummary\"\n        },\n        {\n          \"description\": \"An array of objects, one for each custom data identifier that matches the criteria specified in the request.\"\n        }\n      ]\n    },\n    \"notFoundIdentifierIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array of custom data\
  \ identifier IDs, one for each custom data identifier that was specified in the request but doesn't correlate to an existing custom data identifier.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-batch-get-custom-data-identifiers-response-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BatchGetCustomDataIdentifiersResponse
---
