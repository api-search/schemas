---
description: GetFindingStatisticsRequest schema from Amazon Macie API
layout: schema
name: GetFindingStatisticsRequest
properties_list:
- description: ''
  name: findingCriteria
  type: object
- description: ''
  name: groupBy
  type: object
- description: ''
  name: size
  type: object
- description: ''
  name: sortCriteria
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-finding-statistics-request-schema.json
slug: amazon-macie-get-finding-statistics-request
source_filename: amazon-macie-get-finding-statistics-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-finding-statistics-request-schema.json\",\n  \"title\": \"GetFindingStatisticsRequest\",\n  \"description\": \"GetFindingStatisticsRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findingCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingCriteria\"\n        },\n        {\n          \"description\": \"The criteria to use to filter the query results.\"\n        }\n      ]\n    },\n    \"groupBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupBy\"\n        },\n        {\n          \"description\": \"<p>The finding property to use to group the query results. Valid values are:</p> <ul><li><p>classificationDetails.jobId - The unique identifier for the classification job\
  \ that produced the finding.</p></li> <li><p>resourcesAffected.s3Bucket.name - The name of the S3 bucket that the finding applies to.</p></li> <li><p>severity.description - The severity level of the finding, such as High or Medium.</p></li> <li><p>type - The type of finding, such as Policy:IAMUser/S3BucketPublic and SensitiveData:S3Object/Personal.</p></li></ul>\"\n        }\n      ]\n    },\n    \"size\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The maximum number of items to include in each page of the response.\"\n        }\n      ]\n    },\n    \"sortCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingStatisticsSortCriteria\"\n        },\n        {\n          \"description\": \"The criteria to use to sort the query results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"groupBy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-finding-statistics-request-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetFindingStatisticsRequest
---
