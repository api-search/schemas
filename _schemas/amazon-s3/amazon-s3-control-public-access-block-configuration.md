---
description: The PublicAccessBlock configuration that you want to apply to this Amazon S3 account.
layout: schema
name: PublicAccessBlockConfiguration
properties_list:
- description: Specifies whether Amazon S3 should block public access control lists (ACLs) for buckets in this account.
  name: BlockPublicAcls
  type: boolean
- description: Specifies whether Amazon S3 should ignore public ACLs for buckets in this account.
  name: IgnorePublicAcls
  type: boolean
- description: Specifies whether Amazon S3 should block public bucket policies for buckets in this account.
  name: BlockPublicPolicy
  type: boolean
- description: Specifies whether Amazon S3 should restrict public bucket policies for buckets in this account.
  name: RestrictPublicBuckets
  type: boolean
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-control-public-access-block-configuration-schema.json
slug: amazon-s3-control-public-access-block-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PublicAccessBlockConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"The PublicAccessBlock configuration that you want to apply to this Amazon S3 account.\",\n  \"properties\": {\n    \"BlockPublicAcls\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether Amazon S3 should block public access control lists (ACLs) for buckets in this account.\"\n    },\n    \"IgnorePublicAcls\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether Amazon S3 should ignore public ACLs for buckets in this account.\"\n    },\n    \"BlockPublicPolicy\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether Amazon S3 should block public bucket policies for buckets in this account.\"\n    },\n    \"RestrictPublicBuckets\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether Amazon S3 should restrict public bucket\
  \ policies for buckets in this account.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-control-public-access-block-configuration-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: PublicAccessBlockConfiguration
---
