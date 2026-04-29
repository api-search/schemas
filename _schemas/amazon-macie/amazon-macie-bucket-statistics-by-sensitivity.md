---
description: Provides aggregated statistical data for sensitive data discovery metrics that apply to S3 buckets, grouped by bucket sensitivity score (sensitivityScore). If automated sensitive data discovery is currently disabled for your account, the value for each metric is 0.
layout: schema
name: BucketStatisticsBySensitivity
properties_list:
- description: ''
  name: classificationError
  type: object
- description: ''
  name: notClassified
  type: object
- description: ''
  name: notSensitive
  type: object
- description: ''
  name: sensitive
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-bucket-statistics-by-sensitivity-schema.json
slug: amazon-macie-bucket-statistics-by-sensitivity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-statistics-by-sensitivity-schema.json\",\n  \"title\": \"BucketStatisticsBySensitivity\",\n  \"description\": \"Provides aggregated statistical data for sensitive data discovery metrics that apply to S3 buckets, grouped by bucket sensitivity score (sensitivityScore). If automated sensitive data discovery is currently disabled for your account, the value for each metric is 0.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"classificationError\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitivityAggregations\"\n        },\n        {\n          \"description\": \"The aggregated statistical data for all buckets that have a sensitivity score of -1.\"\n        }\n      ]\n    },\n    \"notClassified\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/SensitivityAggregations\"\n        },\n        {\n          \"description\": \"The aggregated statistical data for all buckets that have a sensitivity score of 50.\"\n        }\n      ]\n    },\n    \"notSensitive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitivityAggregations\"\n        },\n        {\n          \"description\": \"The aggregated statistical data for all buckets that have a sensitivity score of 1-49.\"\n        }\n      ]\n    },\n    \"sensitive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitivityAggregations\"\n        },\n        {\n          \"description\": \"The aggregated statistical data for all buckets that have a sensitivity score of 51-100.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-statistics-by-sensitivity-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BucketStatisticsBySensitivity
---
