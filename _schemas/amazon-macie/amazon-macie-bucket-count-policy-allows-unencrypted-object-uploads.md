---
description: Provides information about the number of S3 buckets whose bucket policies do or don't require server-side encryption of objects when objects are added to the buckets.
layout: schema
name: BucketCountPolicyAllowsUnencryptedObjectUploads
properties_list:
- description: ''
  name: allowsUnencryptedObjectUploads
  type: object
- description: ''
  name: deniesUnencryptedObjectUploads
  type: object
- description: ''
  name: unknown
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-bucket-count-policy-allows-unencrypted-object-uploads-schema.json
slug: amazon-macie-bucket-count-policy-allows-unencrypted-object-uploads
source_filename: amazon-macie-bucket-count-policy-allows-unencrypted-object-uploads-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-count-policy-allows-unencrypted-object-uploads-schema.json\",\n  \"title\": \"BucketCountPolicyAllowsUnencryptedObjectUploads\",\n  \"description\": \"Provides information about the number of S3 buckets whose bucket policies do or don't require server-side encryption of objects when objects are added to the buckets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowsUnencryptedObjectUploads\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets that don't have a bucket policy or have a bucket policy that doesn't require server-side encryption of new objects. If a bucket policy exists, the policy doesn't require PutObject requests to include a valid server-side encryption\
  \ header: the x-amz-server-side-encryption header with a value of AES256 or aws:kms, or the x-amz-server-side-encryption-customer-algorithm header with a value of AES256.\"\n        }\n      ]\n    },\n    \"deniesUnencryptedObjectUploads\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets whose bucket policies require server-side encryption of new objects. PutObject requests for these buckets must include a valid server-side encryption header: the x-amz-server-side-encryption header with a value of AES256 or aws:kms, or the x-amz-server-side-encryption-customer-algorithm header with a value of AES256.\"\n        }\n      ]\n    },\n    \"unknown\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets that Amazon Macie wasn't able to evaluate server-side encryption\
  \ requirements for. Macie can't determine whether the bucket policies for these buckets require server-side encryption of new objects.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-count-policy-allows-unencrypted-object-uploads-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BucketCountPolicyAllowsUnencryptedObjectUploads
---
