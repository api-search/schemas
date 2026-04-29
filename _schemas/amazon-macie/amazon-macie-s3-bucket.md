---
description: Provides information about the S3 bucket that a finding applies to.
layout: schema
name: S3Bucket
properties_list:
- description: ''
  name: allowsUnencryptedObjectUploads
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: defaultServerSideEncryption
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: owner
  type: object
- description: ''
  name: publicAccess
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-s3-bucket-schema.json
slug: amazon-macie-s3-bucket
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-bucket-schema.json\",\n  \"title\": \"S3Bucket\",\n  \"description\": \"Provides information about the S3 bucket that a finding applies to.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowsUnencryptedObjectUploads\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowsUnencryptedObjectUploads\"\n        },\n        {\n          \"description\": \"<p>Specifies whether the bucket policy for the bucket requires server-side encryption of objects when objects are added to the bucket. Possible values are:</p> <ul><li><p>FALSE - The bucket policy requires server-side encryption of new objects. PutObject requests must include a valid server-side encryption header.</p></li> <li><p>TRUE - The bucket doesn't have a bucket policy or it has a bucket policy that\
  \ doesn't require server-side encryption of new objects. If a bucket policy exists, it doesn't require PutObject requests to include a valid server-side encryption header.</p></li> <li><p>UNKNOWN - Amazon Macie can't determine whether the bucket policy requires server-side encryption of new objects.</p></li></ul> <p>Valid server-side encryption headers are: x-amz-server-side-encryption with a value of AES256 or aws:kms, and x-amz-server-side-encryption-customer-algorithm with a value of AES256.</p>\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the bucket.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the\
  \ bucket was created. This value can also indicate when changes such as edits to the bucket's policy were most recently made to the bucket, relative to when the finding was created or last updated.\"\n        }\n      ]\n    },\n    \"defaultServerSideEncryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerSideEncryption\"\n        },\n        {\n          \"description\": \"The default server-side encryption settings for the bucket.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the bucket.\"\n        }\n      ]\n    },\n    \"owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketOwner\"\n        },\n        {\n          \"description\": \"The display name and canonical user ID for the Amazon Web Services account that owns the bucket.\"\n        }\n      ]\n\
  \    },\n    \"publicAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketPublicAccess\"\n        },\n        {\n          \"description\": \"The permissions settings that determine whether the bucket is publicly accessible.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyValuePairList\"\n        },\n        {\n          \"description\": \"The tags that are associated with the bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-bucket-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: S3Bucket
---
