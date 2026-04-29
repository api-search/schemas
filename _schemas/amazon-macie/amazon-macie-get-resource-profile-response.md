---
description: GetResourceProfileResponse schema from Amazon Macie API
layout: schema
name: GetResourceProfileResponse
properties_list:
- description: ''
  name: profileUpdatedAt
  type: object
- description: ''
  name: sensitivityScore
  type: object
- description: ''
  name: sensitivityScoreOverridden
  type: object
- description: ''
  name: statistics
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-resource-profile-response-schema.json
slug: amazon-macie-get-resource-profile-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-resource-profile-response-schema.json\",\n  \"title\": \"GetResourceProfileResponse\",\n  \"description\": \"GetResourceProfileResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profileUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when Amazon Macie most recently recalculated sensitive data discovery statistics and details for the bucket. If the bucket's sensitivity score is calculated automatically, this includes the score.\"\n        }\n      ]\n    },\n    \"sensitivityScore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n      \
  \  },\n        {\n          \"description\": \"The current sensitivity score for the bucket, ranging from -1 (classification error) to 100 (sensitive). By default, this score is calculated automatically based on the amount of data that Amazon Macie has analyzed in the bucket and the amount of sensitive data that Macie has found in the bucket.\"\n        }\n      ]\n    },\n    \"sensitivityScoreOverridden\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the bucket's current sensitivity score was set manually. If this value is true, the score was manually changed to 100. If this value is false, the score was calculated automatically by Amazon Macie.\"\n        }\n      ]\n    },\n    \"statistics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceStatistics\"\n        },\n        {\n          \"description\": \"The sensitive data discovery\
  \ statistics for the bucket. The statistics capture the results of automated sensitive data discovery activities that Amazon Macie has performed for the bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-resource-profile-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetResourceProfileResponse
---
