---
description: Specifies an Amazon Web Services account that owns S3 buckets for a classification job to analyze, and one or more specific buckets to analyze for that account.
layout: schema
name: S3BucketDefinitionForJob
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: buckets
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-s3-bucket-definition-for-job-schema.json
slug: amazon-macie-s3-bucket-definition-for-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-bucket-definition-for-job-schema.json\",\n  \"title\": \"S3BucketDefinitionForJob\",\n  \"description\": \"Specifies an Amazon Web Services account that owns S3 buckets for a classification job to analyze, and one or more specific buckets to analyze for that account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the Amazon Web Services account that owns the buckets.\"\n        }\n      ]\n    },\n    \"buckets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array that lists the names of the buckets.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountId\",\n    \"buckets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-bucket-definition-for-job-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: S3BucketDefinitionForJob
---
