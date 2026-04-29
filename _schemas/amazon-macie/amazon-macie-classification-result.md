---
description: Provides the details of a sensitive data finding, including the types, number of occurrences, and locations of the sensitive data that was detected.
layout: schema
name: ClassificationResult
properties_list:
- description: ''
  name: additionalOccurrences
  type: object
- description: ''
  name: customDataIdentifiers
  type: object
- description: ''
  name: mimeType
  type: object
- description: ''
  name: sensitiveData
  type: object
- description: ''
  name: sizeClassified
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-classification-result-schema.json
slug: amazon-macie-classification-result
source_filename: amazon-macie-classification-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-classification-result-schema.json\",\n  \"title\": \"ClassificationResult\",\n  \"description\": \"Provides the details of a sensitive data finding, including the types, number of occurrences, and locations of the sensitive data that was detected.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalOccurrences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"<p>Specifies whether Amazon Macie detected additional occurrences of sensitive data in the S3 object. A finding includes location data for a maximum of 15 occurrences of sensitive data.</p> <p>This value can help you determine whether to investigate additional occurrences of sensitive data in an object. You can do this by referring\
  \ to the corresponding sensitive data discovery result for the finding (ClassificationDetails.detailedResultsLocation).</p>\"\n        }\n      ]\n    },\n    \"customDataIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomDataIdentifiers\"\n        },\n        {\n          \"description\": \"The custom data identifiers that detected the sensitive data and the number of occurrences of the data that they detected.\"\n        }\n      ]\n    },\n    \"mimeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The type of content, as a MIME type, that the finding applies to. For example, application/gzip, for a GNU Gzip compressed archive file, or application/pdf, for an Adobe Portable Document Format file.\"\n        }\n      ]\n    },\n    \"sensitiveData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveData\"\
  \n        },\n        {\n          \"description\": \"The category, types, and number of occurrences of the sensitive data that produced the finding.\"\n        }\n      ]\n    },\n    \"sizeClassified\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total size, in bytes, of the data that the finding applies to.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassificationResultStatus\"\n        },\n        {\n          \"description\": \"The status of the finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-classification-result-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ClassificationResult
---
