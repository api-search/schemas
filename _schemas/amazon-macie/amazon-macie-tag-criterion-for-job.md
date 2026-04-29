---
description: Specifies a tag-based condition that determines whether an S3 bucket is included or excluded from a classification job.
layout: schema
name: TagCriterionForJob
properties_list:
- description: ''
  name: comparator
  type: object
- description: ''
  name: tagValues
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-tag-criterion-for-job-schema.json
slug: amazon-macie-tag-criterion-for-job
source_filename: amazon-macie-tag-criterion-for-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-tag-criterion-for-job-schema.json\",\n  \"title\": \"TagCriterionForJob\",\n  \"description\": \"Specifies a tag-based condition that determines whether an S3 bucket is included or excluded from a classification job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"comparator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobComparator\"\n        },\n        {\n          \"description\": \"The operator to use in the condition. Valid values are EQ (equals) and NE (not equals).\"\n        }\n      ]\n    },\n    \"tagValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfTagCriterionPairForJob\"\n        },\n        {\n          \"description\": \"The tag keys, tag values, or tag key and value pairs to use in the condition.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-tag-criterion-for-job-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: TagCriterionForJob
---
