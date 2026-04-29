---
description: Specifies property- and tag-based conditions that define criteria for including or excluding S3 buckets from a classification job. Exclude conditions take precedence over include conditions.
layout: schema
name: S3BucketCriteriaForJob
properties_list:
- description: ''
  name: excludes
  type: object
- description: ''
  name: includes
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-s3-bucket-criteria-for-job-schema.json
slug: amazon-macie-s3-bucket-criteria-for-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-bucket-criteria-for-job-schema.json\",\n  \"title\": \"S3BucketCriteriaForJob\",\n  \"description\": \"Specifies property- and tag-based conditions that define criteria for including or excluding S3 buckets from a classification job. Exclude conditions take precedence over include conditions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"excludes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CriteriaBlockForJob\"\n        },\n        {\n          \"description\": \"The property- and tag-based conditions that determine which buckets to exclude from the job.\"\n        }\n      ]\n    },\n    \"includes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CriteriaBlockForJob\"\n        },\n        {\n          \"description\"\
  : \"The property- and tag-based conditions that determine which buckets to include in the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-bucket-criteria-for-job-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: S3BucketCriteriaForJob
---
