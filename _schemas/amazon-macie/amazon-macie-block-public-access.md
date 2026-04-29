---
description: Provides information about the block public access settings for an S3 bucket. These settings can apply to a bucket at the account or bucket level. For detailed information about each setting, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/userguide/access-control-block-public-access.html">Blocking public access to your Amazon S3 storage</a> in the <i>Amazon Simple Storage Service User Guide</i>.
layout: schema
name: BlockPublicAccess
properties_list:
- description: ''
  name: blockPublicAcls
  type: object
- description: ''
  name: blockPublicPolicy
  type: object
- description: ''
  name: ignorePublicAcls
  type: object
- description: ''
  name: restrictPublicBuckets
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-block-public-access-schema.json
slug: amazon-macie-block-public-access
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-block-public-access-schema.json\",\n  \"title\": \"BlockPublicAccess\",\n  \"description\": \"Provides information about the block public access settings for an S3 bucket. These settings can apply to a bucket at the account or bucket level. For detailed information about each setting, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/access-control-block-public-access.html\\\">Blocking public access to your Amazon S3 storage</a> in the <i>Amazon Simple Storage Service User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"blockPublicAcls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether Amazon S3 blocks public access control lists (ACLs) for the\
  \ bucket and objects in the bucket.\"\n        }\n      ]\n    },\n    \"blockPublicPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether Amazon S3 blocks public bucket policies for the bucket.\"\n        }\n      ]\n    },\n    \"ignorePublicAcls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether Amazon S3 ignores public ACLs for the bucket and objects in the bucket.\"\n        }\n      ]\n    },\n    \"restrictPublicBuckets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether Amazon S3 restricts public bucket policies for the bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-block-public-access-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BlockPublicAccess
---
