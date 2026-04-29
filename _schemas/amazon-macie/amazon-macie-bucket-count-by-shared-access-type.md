---
description: Provides information about the number of S3 buckets that are or aren't shared with other Amazon Web Services accounts, Amazon CloudFront origin access identities (OAIs), or CloudFront origin access controls (OACs). In this data, an <i>Amazon Macie organization</i> is defined as a set of Macie accounts that are centrally managed as a group of related accounts through Organizations or by Macie invitation.
layout: schema
name: BucketCountBySharedAccessType
properties_list:
- description: ''
  name: external
  type: object
- description: ''
  name: internal
  type: object
- description: ''
  name: notShared
  type: object
- description: ''
  name: unknown
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-bucket-count-by-shared-access-type-schema.json
slug: amazon-macie-bucket-count-by-shared-access-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-count-by-shared-access-type-schema.json\",\n  \"title\": \"BucketCountBySharedAccessType\",\n  \"description\": \"Provides information about the number of S3 buckets that are or aren't shared with other Amazon Web Services accounts, Amazon CloudFront origin access identities (OAIs), or CloudFront origin access controls (OACs). In this data, an <i>Amazon Macie organization</i> is defined as a set of Macie accounts that are centrally managed as a group of related accounts through Organizations or by Macie invitation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"external\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets that are shared with one or more of the\
  \ following or any combination of the following: an Amazon CloudFront OAI, a CloudFront OAC, or an Amazon Web Services account that isn't in the same Amazon Macie organization.\"\n        }\n      ]\n    },\n    \"internal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets that are shared with one or more Amazon Web Services accounts in the same Amazon Macie organization. These buckets aren't shared with Amazon CloudFront OAIs or OACs.\"\n        }\n      ]\n    },\n    \"notShared\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets that aren't shared with other Amazon Web Services accounts, Amazon CloudFront OAIs, or CloudFront OACs.\"\n        }\n      ]\n    },\n    \"unknown\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\
  \n        },\n        {\n          \"description\": \"The total number of buckets that Amazon Macie wasn't able to evaluate shared access settings for. Macie can't determine whether these buckets are shared with other Amazon Web Services accounts, Amazon CloudFront OAIs, or CloudFront OACs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-count-by-shared-access-type-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BucketCountBySharedAccessType
---
