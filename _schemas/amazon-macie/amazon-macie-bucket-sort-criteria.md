---
description: Specifies criteria for sorting the results of a query for information about S3 buckets.
layout: schema
name: BucketSortCriteria
properties_list:
- description: ''
  name: attributeName
  type: object
- description: ''
  name: orderBy
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-bucket-sort-criteria-schema.json
slug: amazon-macie-bucket-sort-criteria
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-sort-criteria-schema.json\",\n  \"title\": \"BucketSortCriteria\",\n  \"description\": \"Specifies criteria for sorting the results of a query for information about S3 buckets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the bucket property to sort the results by. This value can be one of the following properties that Amazon Macie defines as bucket metadata: accountId, bucketName, classifiableObjectCount, classifiableSizeInBytes, objectCount, sensitivityScore, or sizeInBytes.\"\n        }\n      ]\n    },\n    \"orderBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderBy\"\
  \n        },\n        {\n          \"description\": \"The sort order to apply to the results, based on the value specified by the attributeName property. Valid values are: ASC, sort the results in ascending order; and, DESC, sort the results in descending order.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-sort-criteria-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BucketSortCriteria
---
