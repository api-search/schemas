---
description: <p>Provides statistical data and other information about an S3 bucket that Amazon Macie monitors and analyzes for your account. By default, object count and storage size values include data for object parts that are the result of incomplete multipart uploads. For more information, see <a href="https://docs.aws.amazon.com/macie/latest/user/monitoring-s3-how-it-works.html">How Macie monitors Amazon S3 data security</a> in the <i>Amazon Macie User Guide</i>.</p> <p>If an error occurs when Macie attempts to retrieve and process metadata from Amazon S3 for the bucket or the bucket's objects, the value for the versioning property is false and the value for most other properties is null. Key exceptions are accountId, bucketArn, bucketCreatedAt, bucketName, lastUpdated, and region. To identify the cause of the error, refer to the errorCode and errorMessage values.</p>
layout: schema
name: BucketMetadata
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: allowsUnencryptedObjectUploads
  type: object
- description: ''
  name: bucketArn
  type: object
- description: ''
  name: bucketCreatedAt
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
  name: lastUpdated
  type: object
- description: ''
  name: objectCount
  type: object
- description: ''
  name: objectCountByEncryptionType
  type: object
- description: ''
  name: publicAccess
  type: object
- description: ''
  name: region
  type: object
- description: ''
  name: replicationDetails
  type: object
- description: ''
  name: sensitivityScore
  type: object
- description: ''
  name: serverSideEncryption
  type: object
- description: ''
  name: sharedAccess
  type: object
- description: ''
  name: sizeInBytes
  type: object
- description: ''
  name: sizeInBytesCompressed
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: unclassifiableObjectCount
  type: object
- description: ''
  name: unclassifiableObjectSizeInBytes
  type: object
- description: ''
  name: versioning
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-bucket-metadata-schema.json
slug: amazon-macie-bucket-metadata
source_filename: amazon-macie-bucket-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-metadata-schema.json\",\n  \"title\": \"BucketMetadata\",\n  \"description\": \"<p>Provides statistical data and other information about an S3 bucket that Amazon Macie monitors and analyzes for your account. By default, object count and storage size values include data for object parts that are the result of incomplete multipart uploads. For more information, see <a href=\\\"https://docs.aws.amazon.com/macie/latest/user/monitoring-s3-how-it-works.html\\\">How Macie monitors Amazon S3 data security</a> in the <i>Amazon Macie User Guide</i>.</p> <p>If an error occurs when Macie attempts to retrieve and process metadata from Amazon S3 for the bucket or the bucket's objects, the value for the versioning property is false and the value for most other properties is null. Key exceptions are accountId,\
  \ bucketArn, bucketCreatedAt, bucketName, lastUpdated, and region. To identify the cause of the error, refer to the errorCode and errorMessage values.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the Amazon Web Services account that owns the bucket.\"\n        }\n      ]\n    },\n    \"allowsUnencryptedObjectUploads\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowsUnencryptedObjectUploads\"\n        },\n        {\n          \"description\": \"<p>Specifies whether the bucket policy for the bucket requires server-side encryption of objects when objects are added to the bucket. Possible values are:</p> <ul><li><p>FALSE - The bucket policy requires server-side encryption of new objects. PutObject requests must include a valid server-side encryption header.</p></li>\
  \ <li><p>TRUE - The bucket doesn't have a bucket policy or it has a bucket policy that doesn't require server-side encryption of new objects. If a bucket policy exists, it doesn't require PutObject requests to include a valid server-side encryption header.</p></li> <li><p>UNKNOWN - Amazon Macie can't determine whether the bucket policy requires server-side encryption of new objects.</p></li></ul> <p>Valid server-side encryption headers are: x-amz-server-side-encryption with a value of AES256 or aws:kms, and x-amz-server-side-encryption-customer-algorithm with a value of AES256.</p>\"\n        }\n      ]\n    },\n    \"bucketArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the bucket.\"\n        }\n      ]\n    },\n    \"bucketCreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n      \
  \  {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the bucket was created. This value can also indicate when changes such as edits to the bucket's policy were most recently made to the bucket.\"\n        }\n      ]\n    },\n    \"bucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the bucket.\"\n        }\n      ]\n    },\n    \"classifiableObjectCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of objects that Amazon Macie can analyze in the bucket. These objects use a supported storage class and have a file name extension for a supported file or storage format.\"\n        }\n      ]\n    },\n    \"classifiableSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n   \
  \     },\n        {\n          \"description\": \"<p>The total storage size, in bytes, of the objects that Amazon Macie can analyze in the bucket. These objects use a supported storage class and have a file name extension for a supported file or storage format.</p> <p>If versioning is enabled for the bucket, Macie calculates this value based on the size of the latest version of each applicable object in the bucket. This value doesn't reflect the storage size of all versions of each applicable object in the bucket.</p>\"\n        }\n      ]\n    },\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketMetadataErrorCode\"\n        },\n        {\n          \"description\": \"The error code for an error that prevented Amazon Macie from retrieving and processing information about the bucket and the bucket's objects. If this value is ACCESS_DENIED, Macie doesn't have permission to retrieve the information. For example, the bucket has a restrictive\
  \ bucket policy and Amazon S3 denied the request. If this value is null, Macie was able to retrieve and process the information.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A brief description of the error (errorCode) that prevented Amazon Macie from retrieving and processing information about the bucket and the bucket's objects. This value is null if Macie was able to retrieve and process the information.\"\n        }\n      ]\n    },\n    \"jobDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobDetails\"\n        },\n        {\n          \"description\": \"Specifies whether any one-time or recurring classification jobs are configured to analyze data in the bucket, and, if so, the details of the job that ran most recently.\"\n        }\n      ]\n    },\n    \"lastAutomatedDiscoveryTime\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when Amazon Macie most recently analyzed data in the bucket while performing automated sensitive data discovery for your account. This value is null if automated sensitive data discovery is currently disabled for your account.\"\n        }\n      ]\n    },\n    \"lastUpdated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when Amazon Macie most recently retrieved bucket or object metadata from Amazon S3 for the bucket.\"\n        }\n      ]\n    },\n    \"objectCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of objects\
  \ in the bucket.\"\n        }\n      ]\n    },\n    \"objectCountByEncryptionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectCountByEncryptionType\"\n        },\n        {\n          \"description\": \"The total number of objects in the bucket, grouped by server-side encryption type. This includes a grouping that reports the total number of objects that aren't encrypted or use client-side encryption.\"\n        }\n      ]\n    },\n    \"publicAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketPublicAccess\"\n        },\n        {\n          \"description\": \"Specifies whether the bucket is publicly accessible due to the combination of permissions settings that apply to the bucket, and provides information about those settings.\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\"\
  : \"The Amazon Web Services Region that hosts the bucket.\"\n        }\n      ]\n    },\n    \"replicationDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationDetails\"\n        },\n        {\n          \"description\": \"Specifies whether the bucket is configured to replicate one or more objects to buckets for other Amazon Web Services accounts and, if so, which accounts.\"\n        }\n      ]\n    },\n    \"sensitivityScore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The sensitivity score for the bucket, ranging from -1 (classification error) to 100 (sensitive). This value is null if automated sensitive data discovery is currently disabled for your account.\"\n        }\n      ]\n    },\n    \"serverSideEncryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketServerSideEncryption\"\n        },\n    \
  \    {\n          \"description\": \"The default server-side encryption settings for the bucket.\"\n        }\n      ]\n    },\n    \"sharedAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SharedAccess\"\n        },\n        {\n          \"description\": \"<p>Specifies whether the bucket is shared with another Amazon Web Services account, an Amazon CloudFront origin access identity (OAI), or a CloudFront origin access control (OAC). Possible values are:</p> <ul><li><p>EXTERNAL - The bucket is shared with one or more of the following or any combination of the following: a CloudFront OAI, a CloudFront OAC, or an Amazon Web Services account that isn't part of your Amazon Macie organization.</p></li> <li><p>INTERNAL - The bucket is shared with one or more Amazon Web Services accounts that are part of your Amazon Macie organization. It isn't shared with a CloudFront OAI or OAC.</p></li> <li><p>NOT_SHARED - The bucket isn't shared with another Amazon Web\
  \ Services account, a CloudFront OAI, or a CloudFront OAC.</p></li> <li><p>UNKNOWN - Amazon Macie wasn't able to evaluate the shared access settings for the bucket.</p></li></ul> <p>An <i>Amazon Macie organization</i> is a set of Macie accounts that are centrally managed as a group of related accounts through Organizations or by Macie invitation.</p>\"\n        }\n      ]\n    },\n    \"sizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"<p>The total storage size, in bytes, of the bucket.</p> <p>If versioning is enabled for the bucket, Amazon Macie calculates this value based on the size of the latest version of each object in the bucket. This value doesn't reflect the storage size of all versions of each object in the bucket.</p>\"\n        }\n      ]\n    },\n    \"sizeInBytesCompressed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n       \
  \ },\n        {\n          \"description\": \"<p>The total storage size, in bytes, of the objects that are compressed (.gz, .gzip, .zip) files in the bucket.</p> <p>If versioning is enabled for the bucket, Amazon Macie calculates this value based on the size of the latest version of each applicable object in the bucket. This value doesn't reflect the storage size of all versions of each applicable object in the bucket.</p>\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfKeyValuePair\"\n        },\n        {\n          \"description\": \"An array that specifies the tags (keys and values) that are associated with the bucket.\"\n        }\n      ]\n    },\n    \"unclassifiableObjectCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectLevelStatistics\"\n        },\n        {\n          \"description\": \"The total number of objects that Amazon Macie can't analyze in the\
  \ bucket. These objects don't use a supported storage class or don't have a file name extension for a supported file or storage format.\"\n        }\n      ]\n    },\n    \"unclassifiableObjectSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectLevelStatistics\"\n        },\n        {\n          \"description\": \"The total storage size, in bytes, of the objects that Amazon Macie can't analyze in the bucket. These objects don't use a supported storage class or don't have a file name extension for a supported file or storage format.\"\n        }\n      ]\n    },\n    \"versioning\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether versioning is enabled for the bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-metadata-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BucketMetadata
---
