---
description: Provides information about the number of S3 buckets that are publicly accessible due to a combination of permissions settings for each bucket.
layout: schema
name: BucketCountByEffectivePermission
properties_list:
- description: ''
  name: publiclyAccessible
  type: object
- description: ''
  name: publiclyReadable
  type: object
- description: ''
  name: publiclyWritable
  type: object
- description: ''
  name: unknown
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-bucket-count-by-effective-permission-schema.json
slug: amazon-macie-bucket-count-by-effective-permission
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-count-by-effective-permission-schema.json\",\n  \"title\": \"BucketCountByEffectivePermission\",\n  \"description\": \"Provides information about the number of S3 buckets that are publicly accessible due to a combination of permissions settings for each bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"publiclyAccessible\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets that allow the general public to have read or write access to the bucket.\"\n        }\n      ]\n    },\n    \"publiclyReadable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of\
  \ buckets that allow the general public to have read access to the bucket.\"\n        }\n      ]\n    },\n    \"publiclyWritable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets that allow the general public to have write access to the bucket.\"\n        }\n      ]\n    },\n    \"unknown\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of buckets that Amazon Macie wasn't able to evaluate permissions settings for. Macie can't determine whether these buckets are publicly accessible.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-count-by-effective-permission-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BucketCountByEffectivePermission
---
