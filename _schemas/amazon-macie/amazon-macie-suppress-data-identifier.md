---
description: Specifies a custom data identifier or managed data identifier that detected a type of sensitive data to start excluding or including in an S3 bucket's sensitivity score.
layout: schema
name: SuppressDataIdentifier
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-suppress-data-identifier-schema.json
slug: amazon-macie-suppress-data-identifier
source_filename: amazon-macie-suppress-data-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-suppress-data-identifier-schema.json\",\n  \"title\": \"SuppressDataIdentifier\",\n  \"description\": \"Specifies a custom data identifier or managed data identifier that detected a type of sensitive data to start excluding or including in an S3 bucket's sensitivity score.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the custom data identifier or managed data identifier that detected the type of sensitive data to exclude or include in the score.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataIdentifierType\"\n        },\n        {\n \
  \         \"description\": \"The type of data identifier that detected the sensitive data. Possible values are: CUSTOM, for a custom data identifier; and, MANAGED, for a managed data identifier.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-suppress-data-identifier-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SuppressDataIdentifier
---
