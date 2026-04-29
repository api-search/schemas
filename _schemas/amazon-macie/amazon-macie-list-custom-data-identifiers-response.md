---
description: ListCustomDataIdentifiersResponse schema from Amazon Macie API
layout: schema
name: ListCustomDataIdentifiersResponse
properties_list:
- description: ''
  name: items
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-list-custom-data-identifiers-response-schema.json
slug: amazon-macie-list-custom-data-identifiers-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-custom-data-identifiers-response-schema.json\",\n  \"title\": \"ListCustomDataIdentifiersResponse\",\n  \"description\": \"ListCustomDataIdentifiersResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfCustomDataIdentifierSummary\"\n        },\n        {\n          \"description\": \"An array of objects, one for each custom data identifier.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The string to use in a subsequent request to get the next page of results in a paginated response. This value is null if there are\
  \ no additional pages.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-custom-data-identifiers-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ListCustomDataIdentifiersResponse
---
