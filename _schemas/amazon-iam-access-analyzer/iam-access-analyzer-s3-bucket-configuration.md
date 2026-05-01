---
description: Proposed access control configuration for an Amazon S3 bucket. You can propose a configuration for a new Amazon S3 bucket or an existing Amazon S3 bucket that you own by specifying the Amazon S3 bucket policy, bucket ACLs, bucket BPA settings, Amazon S3 access points, and multi-region access points attached to the bucket. If the configuration is for an existing Amazon S3 bucket and you do not specify the Amazon S3 bucket policy, the access preview uses the existing policy attached to the bucket. If the access preview is for a new resource and you do not specify the Amazon S3 bucket policy, the access preview assumes a bucket without a policy. To propose deletion of an existing bucket policy, you can specify an empty string. For more information about bucket policy limits, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/example-bucket-policies.html">Bucket Policy Examples</a>.
layout: schema
name: S3BucketConfiguration
properties_list:
- description: ''
  name: bucketPolicy
  type: object
- description: ''
  name: bucketAclGrants
  type: object
- description: ''
  name: bucketPublicAccessBlock
  type: object
- description: ''
  name: accessPoints
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-s3-bucket-configuration-schema.json
slug: iam-access-analyzer-s3-bucket-configuration
source_filename: iam-access-analyzer-s3-bucket-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-s3-bucket-configuration-schema.json\",\n  \"title\": \"S3BucketConfiguration\",\n  \"description\": \"Proposed access control configuration for an Amazon S3 bucket. You can propose a configuration for a new Amazon S3 bucket or an existing Amazon S3 bucket that you own by specifying the Amazon S3 bucket policy, bucket ACLs, bucket BPA settings, Amazon S3 access points, and multi-region access points attached to the bucket. If the configuration is for an existing Amazon S3 bucket and you do not specify the Amazon S3 bucket policy, the access preview uses the existing policy attached to the bucket. If the access preview is for a new resource and you do not specify the Amazon S3 bucket policy, the access preview assumes a bucket without a policy. To propose deletion of an existing\
  \ bucket policy, you can specify an empty string. For more information about bucket policy limits, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/example-bucket-policies.html\\\">Bucket Policy Examples</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketPolicy\"\n        },\n        {\n          \"description\": \"The proposed bucket policy for the Amazon S3 bucket.\"\n        }\n      ]\n    },\n    \"bucketAclGrants\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketAclGrantConfigurationsList\"\n        },\n        {\n          \"description\": \"The proposed list of ACL grants for the Amazon S3 bucket. You can propose up to 100 ACL grants per bucket. If the proposed grant configuration is for an existing bucket, the access preview uses the proposed list of grant configurations in place of the existing grants. Otherwise, the\
  \ access preview uses the existing grants for the bucket.\"\n        }\n      ]\n    },\n    \"bucketPublicAccessBlock\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3PublicAccessBlockConfiguration\"\n        },\n        {\n          \"description\": \"The proposed block public access configuration for the Amazon S3 bucket.\"\n        }\n      ]\n    },\n    \"accessPoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3AccessPointConfigurationsMap\"\n        },\n        {\n          \"description\": \"The configuration of Amazon S3 access points or multi-region access points for the bucket. You can propose up to 10 new access points per bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-s3-bucket-configuration-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: S3BucketConfiguration
---
