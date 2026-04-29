---
description: GetBucketStatisticsRequest schema from Amazon Macie API
layout: schema
name: GetBucketStatisticsRequest
properties_list:
- description: ''
  name: accountId
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-bucket-statistics-request-schema.json
slug: amazon-macie-get-bucket-statistics-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-bucket-statistics-request-schema.json\",\n  \"title\": \"GetBucketStatisticsRequest\",\n  \"description\": \"GetBucketStatisticsRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the Amazon Web Services account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-bucket-statistics-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetBucketStatisticsRequest
---
