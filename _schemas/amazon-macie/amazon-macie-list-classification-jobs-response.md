---
description: ListClassificationJobsResponse schema from Amazon Macie API
layout: schema
name: ListClassificationJobsResponse
properties_list:
- description: ''
  name: items
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-list-classification-jobs-response-schema.json
slug: amazon-macie-list-classification-jobs-response
source_filename: amazon-macie-list-classification-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-classification-jobs-response-schema.json\",\n  \"title\": \"ListClassificationJobsResponse\",\n  \"description\": \"ListClassificationJobsResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfJobSummary\"\n        },\n        {\n          \"description\": \"An array of objects, one for each job that matches the filter criteria specified in the request.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The string to use in a subsequent request to get the next page of results in a paginated response. This value is null\
  \ if there are no additional pages.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-classification-jobs-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ListClassificationJobsResponse
---
