---
description: Specifies a property- or tag-based condition that defines criteria for including or excluding S3 buckets from a classification job.
layout: schema
name: CriteriaForJob
properties_list:
- description: ''
  name: simpleCriterion
  type: object
- description: ''
  name: tagCriterion
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-criteria-for-job-schema.json
slug: amazon-macie-criteria-for-job
source_filename: amazon-macie-criteria-for-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-criteria-for-job-schema.json\",\n  \"title\": \"CriteriaForJob\",\n  \"description\": \"Specifies a property- or tag-based condition that defines criteria for including or excluding S3 buckets from a classification job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"simpleCriterion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimpleCriterionForJob\"\n        },\n        {\n          \"description\": \"A property-based condition that defines a property, operator, and one or more values for including or excluding buckets from the job.\"\n        }\n      ]\n    },\n    \"tagCriterion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagCriterionForJob\"\n        },\n        {\n          \"description\": \"A tag-based condition\
  \ that defines an operator and tag keys, tag values, or tag key and value pairs for including or excluding buckets from the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-criteria-for-job-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: CriteriaForJob
---
