---
description: Provides statistical data for sensitive data discovery metrics that apply to an S3 bucket that Amazon Macie monitors and analyzes for your account. The statistics capture the results of automated sensitive data discovery activities that Macie has performed for the bucket. The data is available only if automated sensitive data discovery is currently enabled for your account.
layout: schema
name: ResourceStatistics
properties_list:
- description: ''
  name: totalBytesClassified
  type: object
- description: ''
  name: totalDetections
  type: object
- description: ''
  name: totalDetectionsSuppressed
  type: object
- description: ''
  name: totalItemsClassified
  type: object
- description: ''
  name: totalItemsSensitive
  type: object
- description: ''
  name: totalItemsSkipped
  type: object
- description: ''
  name: totalItemsSkippedInvalidEncryption
  type: object
- description: ''
  name: totalItemsSkippedInvalidKms
  type: object
- description: ''
  name: totalItemsSkippedPermissionDenied
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-resource-statistics-schema.json
slug: amazon-macie-resource-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-resource-statistics-schema.json\",\n  \"title\": \"ResourceStatistics\",\n  \"description\": \"Provides statistical data for sensitive data discovery metrics that apply to an S3 bucket that Amazon Macie monitors and analyzes for your account. The statistics capture the results of automated sensitive data discovery activities that Macie has performed for the bucket. The data is available only if automated sensitive data discovery is currently enabled for your account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalBytesClassified\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total amount of data, in bytes, that Amazon Macie has analyzed in the bucket.\"\n        }\n      ]\n    },\n\
  \    \"totalDetections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of occurrences of sensitive data that Amazon Macie has found in the bucket's objects. This includes occurrences that are currently suppressed by the sensitivity scoring settings for the bucket (totalDetectionsSuppressed).\"\n        }\n      ]\n    },\n    \"totalDetectionsSuppressed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of occurrences of sensitive data that are currently suppressed by the sensitivity scoring settings for the bucket. These represent occurrences of sensitive data that Amazon Macie found in the bucket's objects, but the occurrences were manually suppressed. By default, suppressed occurrences are excluded from the bucket's sensitivity score.\"\n        }\n      ]\n    },\n \
  \   \"totalItemsClassified\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of objects that Amazon Macie has analyzed in the bucket.\"\n        }\n      ]\n    },\n    \"totalItemsSensitive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of the bucket's objects that Amazon Macie has found sensitive data in.\"\n        }\n      ]\n    },\n    \"totalItemsSkipped\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"<p>The total number of objects that Amazon Macie hasn't analyzed in the bucket due to an error or issue. For example, the object is a malformed file. This value includes objects that Macie hasn't analyzed for reasons reported by other statistics in the ResourceStatistics object.</p>\
  \ \"\n        }\n      ]\n    },\n    \"totalItemsSkippedInvalidEncryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of objects that Amazon Macie hasn't analyzed in the bucket because the objects are encrypted with a key that Macie isn't allowed to use.\"\n        }\n      ]\n    },\n    \"totalItemsSkippedInvalidKms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of objects that Amazon Macie hasn't analyzed in the bucket because the objects are encrypted with an KMS key that was disabled or deleted.\"\n        }\n      ]\n    },\n    \"totalItemsSkippedPermissionDenied\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of objects that Amazon Macie hasn't\
  \ analyzed in the bucket because Macie isn't allowed to access the objects.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-resource-statistics-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ResourceStatistics
---
