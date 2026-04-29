---
description: A proposed access control list grant configuration for an Amazon S3 bucket. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/acl-overview.html#setting-acls">How to Specify an ACL</a>.
layout: schema
name: S3BucketAclGrantConfiguration
properties_list:
- description: ''
  name: permission
  type: object
- description: ''
  name: grantee
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-s3-bucket-acl-grant-configuration-schema.json
slug: iam-access-analyzer-s3-bucket-acl-grant-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-s3-bucket-acl-grant-configuration-schema.json\",\n  \"title\": \"S3BucketAclGrantConfiguration\",\n  \"description\": \"A proposed access control list grant configuration for an Amazon S3 bucket. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/acl-overview.html#setting-acls\\\">How to Specify an ACL</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permission\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AclPermission\"\n        },\n        {\n          \"description\": \"The permissions being granted.\"\n        }\n      ]\n    },\n    \"grantee\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AclGrantee\"\n        },\n        {\n          \"description\": \"\
  The grantee to whom you\\u2019re assigning access rights.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"permission\",\n    \"grantee\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-s3-bucket-acl-grant-configuration-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: S3BucketAclGrantConfiguration
---
