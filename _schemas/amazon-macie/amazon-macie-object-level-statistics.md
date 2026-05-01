---
description: Provides information about the total storage size (in bytes) or number of objects that Amazon Macie can't analyze in one or more S3 buckets. In a BucketMetadata or MatchingBucket object, this data is for a specific bucket. In a GetBucketStatisticsResponse object, this data is aggregated for all the buckets in the query results. If versioning is enabled for a bucket, storage size values are based on the size of the latest version of each applicable object in the bucket.
layout: schema
name: ObjectLevelStatistics
properties_list:
- description: ''
  name: fileType
  type: object
- description: ''
  name: storageClass
  type: object
- description: ''
  name: total
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-object-level-statistics-schema.json
slug: amazon-macie-object-level-statistics
source_filename: amazon-macie-object-level-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-object-level-statistics-schema.json\",\n  \"title\": \"ObjectLevelStatistics\",\n  \"description\": \"Provides information about the total storage size (in bytes) or number of objects that Amazon Macie can't analyze in one or more S3 buckets. In a BucketMetadata or MatchingBucket object, this data is for a specific bucket. In a GetBucketStatisticsResponse object, this data is aggregated for all the buckets in the query results. If versioning is enabled for a bucket, storage size values are based on the size of the latest version of each applicable object in the bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total storage size\
  \ (in bytes) or number of objects that Amazon Macie can't analyze because the objects don't have a file name extension for a supported file or storage format.\"\n        }\n      ]\n    },\n    \"storageClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total storage size (in bytes) or number of objects that Amazon Macie can't analyze because the objects use an unsupported storage class.\"\n        }\n      ]\n    },\n    \"total\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total storage size (in bytes) or number of objects that Amazon Macie can't analyze because the objects use an unsupported storage class or don't have a file name extension for a supported file or storage format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-object-level-statistics-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ObjectLevelStatistics
---
