---
description: 'The property to use in a condition that determines whether an S3 bucket is included or excluded from a classification job. Valid values are:'
layout: schema
name: SimpleCriterionKeyForJob
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-simple-criterion-key-for-job-schema.json
slug: amazon-macie-simple-criterion-key-for-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-simple-criterion-key-for-job-schema.json\",\n  \"title\": \"SimpleCriterionKeyForJob\",\n  \"description\": \"The property to use in a condition that determines whether an S3 bucket is included or excluded from a classification job. Valid values are:\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ACCOUNT_ID\",\n    \"S3_BUCKET_NAME\",\n    \"S3_BUCKET_EFFECTIVE_PERMISSION\",\n    \"S3_BUCKET_SHARED_ACCESS\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-simple-criterion-key-for-job-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SimpleCriterionKeyForJob
---
