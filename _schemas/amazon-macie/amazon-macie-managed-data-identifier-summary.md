---
description: Provides information about a managed data identifier. For additional information, see <a href="https://docs.aws.amazon.com/macie/latest/user/managed-data-identifiers.html">Using managed data identifiers</a> in the <i>Amazon Macie User Guide</i>.
layout: schema
name: ManagedDataIdentifierSummary
properties_list:
- description: ''
  name: category
  type: object
- description: ''
  name: id
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-managed-data-identifier-summary-schema.json
slug: amazon-macie-managed-data-identifier-summary
source_filename: amazon-macie-managed-data-identifier-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-managed-data-identifier-summary-schema.json\",\n  \"title\": \"ManagedDataIdentifierSummary\",\n  \"description\": \"Provides information about a managed data identifier. For additional information, see <a href=\\\"https://docs.aws.amazon.com/macie/latest/user/managed-data-identifiers.html\\\">Using managed data identifiers</a> in the <i>Amazon Macie User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveDataItemCategory\"\n        },\n        {\n          \"description\": \"The category of sensitive data that the managed data identifier detects: CREDENTIALS, for credentials data such as private keys or Amazon Web Services secret access keys; FINANCIAL_INFORMATION, for financial\
  \ data such as credit card numbers; or, PERSONAL_INFORMATION, for personal health information, such as health insurance identification numbers, or personally identifiable information, such as passport numbers.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the managed data identifier. This is a string that describes the type of sensitive data that the managed data identifier detects. For example: OPENSSH_PRIVATE_KEY for OpenSSH private keys, CREDIT_CARD_NUMBER for credit card numbers, or USA_PASSPORT_NUMBER for US passport numbers.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-managed-data-identifier-summary-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ManagedDataIdentifierSummary
---
