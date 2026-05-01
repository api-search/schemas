---
description: Provides aggregated statistical data for sensitive data discovery metrics that apply to S3 buckets. Each field contains aggregated data for all the buckets that have a sensitivity score (sensitivityScore) of a specified value or within a specified range (BucketStatisticsBySensitivity). If automated sensitive data discovery is currently disabled for your account, the value for each field is 0.
layout: schema
name: SensitivityAggregations
properties_list:
- description: ''
  name: classifiableSizeInBytes
  type: object
- description: ''
  name: publiclyAccessibleCount
  type: object
- description: ''
  name: totalCount
  type: object
- description: ''
  name: totalSizeInBytes
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-sensitivity-aggregations-schema.json
slug: amazon-macie-sensitivity-aggregations
source_filename: amazon-macie-sensitivity-aggregations-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitivity-aggregations-schema.json\",\n  \"title\": \"SensitivityAggregations\",\n  \"description\": \"Provides aggregated statistical data for sensitive data discovery metrics that apply to S3 buckets. Each field contains aggregated data for all the buckets that have a sensitivity score (sensitivityScore) of a specified value or within a specified range (BucketStatisticsBySensitivity). If automated sensitive data discovery is currently disabled for your account, the value for each field is 0.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"classifiableSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"<p>The total storage size, in bytes, of all the objects that Amazon Macie can analyze\
  \ in the buckets. These objects use a supported storage class and have a file name extension for a supported file or storage format.</p> <p>If versioning is enabled for any of the buckets, this value is based on the size of the latest version of each applicable object in the buckets. This value doesn't reflect the storage size of all versions of all applicable objects in the buckets.</p>\"\n        }\n      ]\n    },\n    \"publiclyAccessibleCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets that are publicly accessible due to a combination of permissions settings for each bucket.\"\n        }\n      ]\n    },\n    \"totalCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets.\"\n        }\n      ]\n    },\n    \"totalSizeInBytes\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"<p>The total storage size, in bytes, of the buckets.</p> <p>If versioning is enabled for any of the buckets, this value is based on the size of the latest version of each object in the buckets. This value doesn't reflect the storage size of all versions of the objects in the buckets.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-sensitivity-aggregations-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SensitivityAggregations
---
