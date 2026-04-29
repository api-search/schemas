---
description: UpdateResourceProfileRequest schema from Amazon Macie API
layout: schema
name: UpdateResourceProfileRequest
properties_list:
- description: ''
  name: sensitivityScoreOverride
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-update-resource-profile-request-schema.json
slug: amazon-macie-update-resource-profile-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-resource-profile-request-schema.json\",\n  \"title\": \"UpdateResourceProfileRequest\",\n  \"description\": \"UpdateResourceProfileRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sensitivityScoreOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The new sensitivity score for the bucket. Valid values are: 100, assign the maximum score and apply the <i>Sensitive</i> label to the bucket; and, null (empty), assign a score that Amazon Macie calculates automatically after you submit the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-resource-profile-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UpdateResourceProfileRequest
---
