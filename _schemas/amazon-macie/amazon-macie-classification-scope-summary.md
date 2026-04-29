---
description: Provides information about the classification scope for an Amazon Macie account. Macie uses the scope's settings when it performs automated sensitive data discovery for the account.
layout: schema
name: ClassificationScopeSummary
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-classification-scope-summary-schema.json
slug: amazon-macie-classification-scope-summary
source_filename: amazon-macie-classification-scope-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-classification-scope-summary-schema.json\",\n  \"title\": \"ClassificationScopeSummary\",\n  \"description\": \"Provides information about the classification scope for an Amazon Macie account. Macie uses the scope's settings when it performs automated sensitive data discovery for the account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassificationScopeId\"\n        },\n        {\n          \"description\": \"The unique identifier for the classification scope.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassificationScopeName\"\n        },\n        {\n          \"description\": \"The name of the classification scope: automated-sensitive-data-discovery.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-classification-scope-summary-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ClassificationScopeSummary
---
