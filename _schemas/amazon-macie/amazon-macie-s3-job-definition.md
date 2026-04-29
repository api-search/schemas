---
description: Specifies which S3 buckets contain the objects that a classification job analyzes, and the scope of that analysis. The bucket specification can be static (bucketDefinitions) or dynamic (bucketCriteria). If it's static, the job analyzes objects in the same predefined set of buckets each time the job runs. If it's dynamic, the job analyzes objects in any buckets that match the specified criteria each time the job starts to run.
layout: schema
name: S3JobDefinition
properties_list:
- description: ''
  name: bucketCriteria
  type: object
- description: ''
  name: bucketDefinitions
  type: object
- description: ''
  name: scoping
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-s3-job-definition-schema.json
slug: amazon-macie-s3-job-definition
source_filename: amazon-macie-s3-job-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-job-definition-schema.json\",\n  \"title\": \"S3JobDefinition\",\n  \"description\": \"Specifies which S3 buckets contain the objects that a classification job analyzes, and the scope of that analysis. The bucket specification can be static (bucketDefinitions) or dynamic (bucketCriteria). If it's static, the job analyzes objects in the same predefined set of buckets each time the job runs. If it's dynamic, the job analyzes objects in any buckets that match the specified criteria each time the job starts to run.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketCriteriaForJob\"\n        },\n        {\n          \"description\": \"The property- and tag-based conditions that determine\
  \ which S3 buckets to include or exclude from the analysis. Each time the job runs, the job uses these criteria to determine which buckets contain objects to analyze. A job's definition can contain a bucketCriteria object or a bucketDefinitions array, not both.\"\n        }\n      ]\n    },\n    \"bucketDefinitions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfS3BucketDefinitionForJob\"\n        },\n        {\n          \"description\": \"An array of objects, one for each Amazon Web Services account that owns specific S3 buckets to analyze. Each object specifies the account ID for an account and one or more buckets to analyze for that account. A job's definition can contain a bucketDefinitions array or a bucketCriteria object, not both.\"\n        }\n      ]\n    },\n    \"scoping\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scoping\"\n        },\n        {\n          \"description\": \"The property- and tag-based\
  \ conditions that determine which S3 objects to include or exclude from the analysis. Each time the job runs, the job uses these criteria to determine which objects to analyze.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-job-definition-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: S3JobDefinition
---
