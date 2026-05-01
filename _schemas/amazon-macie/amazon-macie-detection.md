---
description: Provides information about a type of sensitive data that Amazon Macie found in an S3 bucket while performing automated sensitive data discovery for the bucket. The information also specifies the custom data identifier or managed data identifier that detected the data. This information is available only if automated sensitive data discovery is currently enabled for your account.
layout: schema
name: Detection
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: count
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: suppressed
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-detection-schema.json
slug: amazon-macie-detection
source_filename: amazon-macie-detection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-detection-schema.json\",\n  \"title\": \"Detection\",\n  \"description\": \"Provides information about a type of sensitive data that Amazon Macie found in an S3 bucket while performing automated sensitive data discovery for the bucket. The information also specifies the custom data identifier or managed data identifier that detected the data. This information is available only if automated sensitive data discovery is currently enabled for your account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"If the sensitive data was detected by a custom data identifier, the Amazon Resource Name (ARN) of the custom data identifier that detected the\
  \ data. Otherwise, this value is null.\"\n        }\n      ]\n    },\n    \"count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of occurrences of the sensitive data.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the custom data identifier or managed data identifier that detected the sensitive data. For additional details about a specified managed data identifier, see <a href=\\\"https://docs.aws.amazon.com/macie/latest/user/managed-data-identifiers.html\\\">Using managed data identifiers</a> in the <i>Amazon Macie User Guide</i>.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"\
  The name of the custom data identifier or managed data identifier that detected the sensitive data. For a managed data identifier, this value is the same as the unique identifier (id).\"\n        }\n      ]\n    },\n    \"suppressed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether occurrences of this type of sensitive data are excluded (true) or included (false) in the bucket's sensitivity score.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataIdentifierType\"\n        },\n        {\n          \"description\": \"The type of data identifier that detected the sensitive data. Possible values are: CUSTOM, for a custom data identifier; and, MANAGED, for a managed data identifier.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-detection-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: Detection
---
