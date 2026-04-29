---
description: <p>Container for granting information.</p> <p>Buckets that use the bucket owner enforced setting for Object Ownership don't support target grants. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/userguide/enable-server-access-logging.html#grant-log-delivery-permissions-general">Permissions server access log delivery</a> in the <i>Amazon S3 User Guide</i>.</p>
layout: schema
name: TargetGrant
properties_list:
- description: ''
  name: Grantee
  type: object
- description: ''
  name: Permission
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-targetgrant-schema.json
slug: s3-targetgrant
source_filename: s3-targetgrant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TargetGrant\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Grantee\": {},\n    \"Permission\": {}\n  },\n  \"description\": \"<p>Container for granting information.</p> <p>Buckets that use the bucket owner enforced setting for Object Ownership don't support target grants. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/enable-server-access-logging.html#grant-log-delivery-permissions-general\\\">Permissions server access log delivery</a> in the <i>Amazon S3 User Guide</i>.</p>\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-targetgrant-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: TargetGrant
---
