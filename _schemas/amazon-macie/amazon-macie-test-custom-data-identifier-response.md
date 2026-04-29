---
description: TestCustomDataIdentifierResponse schema from Amazon Macie API
layout: schema
name: TestCustomDataIdentifierResponse
properties_list:
- description: ''
  name: matchCount
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-test-custom-data-identifier-response-schema.json
slug: amazon-macie-test-custom-data-identifier-response
source_filename: amazon-macie-test-custom-data-identifier-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-test-custom-data-identifier-response-schema.json\",\n  \"title\": \"TestCustomDataIdentifierResponse\",\n  \"description\": \"TestCustomDataIdentifierResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"matchCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The number of occurrences of sample text that matched the criteria specified by the custom data identifier.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-test-custom-data-identifier-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: TestCustomDataIdentifierResponse
---
