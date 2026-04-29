---
description: <p>Provides statistical data and other information about an S3 bucket that Amazon Macie monitors and analyzes for your account. By default, object count and storage size values include data for object parts that are the result of incomplete multipart uploads. For more information, see <a href="https://docs.aws.amazon.com/macie/latest/user/monitoring-s3-how-it-works.html">How Macie monitors Amazon S3 data security</a> in the <i>Amazon Macie User Guide</i>.</p> <p>If an error occurs when Macie attempts to retrieve and process information about the bucket or the bucket's objects, the value for most of these properties is null. Key exceptions are accountId and bucketName. To identify the cause of the error, refer to the errorCode and errorMessage values.</p>
layout: schema
name: MatchingBucket
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: bucketName
  type: object
- description: ''
  name: classifiableObjectCount
  type: object
- description: ''
  name: classifiableSizeInBytes
  type: object
- description: ''
  name: errorCode
  type: object
- description: ''
  name: errorMessage
  type: object
- description: ''
  name: jobDetails
  type: object
- description: ''
  name: lastAutomatedDiscoveryTime
  type: object
- description: ''
  name: objectCount
  type: object
- description: ''
  name: objectCountByEncryptionType
  type: object
- description: ''
  name: sensitivityScore
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
schema_file: json-schema/amazon-macie-matching-bucket-schema.json
slug: amazon-macie-matching-bucket
source_filename: amazon-macie-matching-bucket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-matching-bucket-schema.json\",\n  \"title\": \"MatchingBucket\",\n  \"description\": \"<p>Provides statistical data and other information about an S3 bucket that Amazon Macie monitors and analyzes for your account. By default, object count and storage size values include data for object parts that are the result of incomplete multipart uploads. For more information, see <a href=\\\"https://docs.aws.amazon.com/macie/latest/user/monitoring-s3-how-it-works.html\\\">How Macie monitors Amazon S3 data security</a> in the <i>Amazon Macie User Guide</i>.</p> <p>If an error occurs when Macie attempts to retrieve and process information about the bucket or the bucket's objects, the value for most of these properties is null. Key exceptions are accountId and bucketName. To identify the cause of the error,\
  \ refer to the errorCode and errorMessage values.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the Amazon Web Services account that owns the bucket.\"\n        }\n      ]\n    },\n    \"bucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the bucket.\"\n        }\n      ]\n    },\n    \"classifiableObjectCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of objects that Amazon Macie can analyze in the bucket. These objects use a supported storage class and have a file name extension for a supported file or storage format.\"\n        }\n      ]\n    },\n    \"classifiableSizeInBytes\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"<p>The total storage size, in bytes, of the objects that Amazon Macie can analyze in the bucket. These objects use a supported storage class and have a file name extension for a supported file or storage format.</p> <p>If versioning is enabled for the bucket, Macie calculates this value based on the size of the latest version of each applicable object in the bucket. This value doesn't reflect the storage size of all versions of each applicable object in the bucket.</p>\"\n        }\n      ]\n    },\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketMetadataErrorCode\"\n        },\n        {\n          \"description\": \"The error code for an error that prevented Amazon Macie from retrieving and processing information about the bucket and the bucket's objects. If this value is ACCESS_DENIED, Macie\
  \ doesn't have permission to retrieve the information. For example, the bucket has a restrictive bucket policy and Amazon S3 denied the request. If this value is null, Macie was able to retrieve and process the information.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A brief description of the error (errorCode) that prevented Amazon Macie from retrieving and processing information about the bucket and the bucket's objects. This value is null if Macie was able to retrieve and process the information.\"\n        }\n      ]\n    },\n    \"jobDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobDetails\"\n        },\n        {\n          \"description\": \"Specifies whether any one-time or recurring classification jobs are configured to analyze objects in the bucket, and, if so, the details of the job that\
  \ ran most recently.\"\n        }\n      ]\n    },\n    \"lastAutomatedDiscoveryTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when Amazon Macie most recently analyzed data in the bucket while performing automated sensitive data discovery for your account. This value is null if automated sensitive data discovery is currently disabled for your account.\"\n        }\n      ]\n    },\n    \"objectCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of objects in the bucket.\"\n        }\n      ]\n    },\n    \"objectCountByEncryptionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectCountByEncryptionType\"\n        },\n        {\n          \"description\": \"The total number\
  \ of objects in the bucket, grouped by server-side encryption type. This includes a grouping that reports the total number of objects that aren't encrypted or use client-side encryption.\"\n        }\n      ]\n    },\n    \"sensitivityScore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The current sensitivity score for the bucket, ranging from -1 (classification error) to 100 (sensitive). This value is null if automated sensitive data discovery is currently disabled for your account.\"\n        }\n      ]\n    },\n    \"sizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"<p>The total storage size, in bytes, of the bucket.</p> <p>If versioning is enabled for the bucket, Amazon Macie calculates this value based on the size of the latest version of each object in the bucket. This value doesn't\
  \ reflect the storage size of all versions of each object in the bucket.</p>\"\n        }\n      ]\n    },\n    \"sizeInBytesCompressed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"<p>The total storage size, in bytes, of the objects that are compressed (.gz, .gzip, .zip) files in the bucket.</p> <p>If versioning is enabled for the bucket, Amazon Macie calculates this value based on the size of the latest version of each applicable object in the bucket. This value doesn't reflect the storage size of all versions of each applicable object in the bucket.</p>\"\n        }\n      ]\n    },\n    \"unclassifiableObjectCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectLevelStatistics\"\n        },\n        {\n          \"description\": \"The total number of objects that Amazon Macie can't analyze in the bucket. These objects don't use a supported storage class\
  \ or don't have a file name extension for a supported file or storage format.\"\n        }\n      ]\n    },\n    \"unclassifiableObjectSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectLevelStatistics\"\n        },\n        {\n          \"description\": \"The total storage size, in bytes, of the objects that Amazon Macie can't analyze in the bucket. These objects don't use a supported storage class or don't have a file name extension for a supported file or storage format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-matching-bucket-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: MatchingBucket
---
