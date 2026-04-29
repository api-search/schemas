---
description: SearchResourcesRequest schema from Amazon Macie API
layout: schema
name: SearchResourcesRequest
properties_list:
- description: ''
  name: bucketCriteria
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
schema_file: json-schema/amazon-macie-search-resources-request-schema.json
slug: amazon-macie-search-resources-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-search-resources-request-schema.json\",\n  \"title\": \"SearchResourcesRequest\",\n  \"description\": \"SearchResourcesRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchResourcesBucketCriteria\"\n        },\n        {\n          \"description\": \"The filter conditions that determine which S3 buckets to include or exclude from the query results.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The maximum number of items to include in each page of the response. The default value is 50.\"\n        }\n      ]\n\
  \    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The nextToken string that specifies which page of results to return in a paginated response.\"\n        }\n      ]\n    },\n    \"sortCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchResourcesSortCriteria\"\n        },\n        {\n          \"description\": \"The criteria to use to sort the results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-search-resources-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: SearchResourcesRequest
---
