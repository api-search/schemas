---
description: GetBucketStatisticsResponse schema from Amazon Macie API
layout: schema
name: GetBucketStatisticsResponse
properties_list:
- description: ''
  name: bucketCount
  type: object
- description: ''
  name: bucketCountByEffectivePermission
  type: object
- description: ''
  name: bucketCountByEncryptionType
  type: object
- description: ''
  name: bucketCountByObjectEncryptionRequirement
  type: object
- description: ''
  name: bucketCountBySharedAccessType
  type: object
- description: ''
  name: bucketStatisticsBySensitivity
  type: object
- description: ''
  name: classifiableObjectCount
  type: object
- description: ''
  name: classifiableSizeInBytes
  type: object
- description: ''
  name: lastUpdated
  type: object
- description: ''
  name: objectCount
  type: object
- description: ''
  name: sizeInBytes
  type: object
- description: ''
  name: sizeInBytesCompressed
  type: object
- description: ''
  name: unclassifiableObjectCount
  type: object
- description: ''
  name: unclassifiableObjectSizeInBytes
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-bucket-statistics-response-schema.json
slug: amazon-macie-get-bucket-statistics-response
source_filename: amazon-macie-get-bucket-statistics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-bucket-statistics-response-schema.json\",\n  \"title\": \"GetBucketStatisticsResponse\",\n  \"description\": \"GetBucketStatisticsResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets.\"\n        }\n      ]\n    },\n    \"bucketCountByEffectivePermission\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketCountByEffectivePermission\"\n        },\n        {\n          \"description\": \"The total number of buckets that are publicly accessible due to a combination of permissions settings for each bucket.\"\n        }\n      ]\n    },\n   \
  \ \"bucketCountByEncryptionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketCountByEncryptionType\"\n        },\n        {\n          \"description\": \"The total number of buckets whose settings do or don't specify default server-side encryption behavior for objects that are added to the buckets.\"\n        }\n      ]\n    },\n    \"bucketCountByObjectEncryptionRequirement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketCountPolicyAllowsUnencryptedObjectUploads\"\n        },\n        {\n          \"description\": \"The total number of buckets whose bucket policies do or don't require server-side encryption of objects when objects are added to the buckets.\"\n        }\n      ]\n    },\n    \"bucketCountBySharedAccessType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketCountBySharedAccessType\"\n        },\n        {\n          \"description\": \"The total number of buckets\
  \ that are or aren't shared with other Amazon Web Services accounts, Amazon CloudFront origin access identities (OAIs), or CloudFront origin access controls (OACs).\"\n        }\n      ]\n    },\n    \"bucketStatisticsBySensitivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketStatisticsBySensitivity\"\n        },\n        {\n          \"description\": \"The aggregated sensitive data discovery statistics for the buckets. If automated sensitive data discovery is currently disabled for your account, the value for each statistic is 0.\"\n        }\n      ]\n    },\n    \"classifiableObjectCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of objects that Amazon Macie can analyze in the buckets. These objects use a supported storage class and have a file name extension for a supported file or storage format.\"\n        }\n      ]\n    },\n\
  \    \"classifiableSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"<p>The total storage size, in bytes, of all the objects that Amazon Macie can analyze in the buckets. These objects use a supported storage class and have a file name extension for a supported file or storage format.</p> <p>If versioning is enabled for any of the buckets, this value is based on the size of the latest version of each applicable object in the buckets. This value doesn't reflect the storage size of all versions of all applicable objects in the buckets.</p>\"\n        }\n      ]\n    },\n    \"lastUpdated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when Amazon Macie most recently retrieved bucket or object metadata from Amazon S3 for the buckets.\"\
  \n        }\n      ]\n    },\n    \"objectCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of objects in the buckets.\"\n        }\n      ]\n    },\n    \"sizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"<p>The total storage size, in bytes, of the buckets.</p> <p>If versioning is enabled for any of the buckets, this value is based on the size of the latest version of each object in the buckets. This value doesn't reflect the storage size of all versions of the objects in the buckets.</p>\"\n        }\n      ]\n    },\n    \"sizeInBytesCompressed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"<p>The total storage size, in bytes, of the objects that are compressed (.gz, .gzip,\
  \ .zip) files in the buckets.</p> <p>If versioning is enabled for any of the buckets, this value is based on the size of the latest version of each applicable object in the buckets. This value doesn't reflect the storage size of all versions of the applicable objects in the buckets.</p>\"\n        }\n      ]\n    },\n    \"unclassifiableObjectCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectLevelStatistics\"\n        },\n        {\n          \"description\": \"The total number of objects that Amazon Macie can't analyze in the buckets. These objects don't use a supported storage class or don't have a file name extension for a supported file or storage format.\"\n        }\n      ]\n    },\n    \"unclassifiableObjectSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectLevelStatistics\"\n        },\n        {\n          \"description\": \"The total storage size, in bytes, of the objects that Amazon Macie\
  \ can't analyze in the buckets. These objects don't use a supported storage class or don't have a file name extension for a supported file or storage format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-bucket-statistics-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetBucketStatisticsResponse
---
