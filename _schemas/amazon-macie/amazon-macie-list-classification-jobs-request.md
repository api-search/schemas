---
description: ListClassificationJobsRequest schema from Amazon Macie API
layout: schema
name: ListClassificationJobsRequest
properties_list:
- description: ''
  name: filterCriteria
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: sortCriteria
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-list-classification-jobs-request-schema.json
slug: amazon-macie-list-classification-jobs-request
source_filename: amazon-macie-list-classification-jobs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-classification-jobs-request-schema.json\",\n  \"title\": \"ListClassificationJobsRequest\",\n  \"description\": \"ListClassificationJobsRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filterCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListJobsFilterCriteria\"\n        },\n        {\n          \"description\": \"The criteria to use to filter the results.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The maximum number of items to include in each page of the response.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The nextToken string that specifies which page of results to return in a paginated response.\"\n        }\n      ]\n    },\n    \"sortCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListJobsSortCriteria\"\n        },\n        {\n          \"description\": \"The criteria to use to sort the results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-classification-jobs-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ListClassificationJobsRequest
---
