---
description: Specifies criteria for filtering the results of a request for information about classification jobs.
layout: schema
name: ListJobsFilterCriteria
properties_list:
- description: ''
  name: excludes
  type: object
- description: ''
  name: includes
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-list-jobs-filter-criteria-schema.json
slug: amazon-macie-list-jobs-filter-criteria
source_filename: amazon-macie-list-jobs-filter-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-jobs-filter-criteria-schema.json\",\n  \"title\": \"ListJobsFilterCriteria\",\n  \"description\": \"Specifies criteria for filtering the results of a request for information about classification jobs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"excludes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfListJobsFilterTerm\"\n        },\n        {\n          \"description\": \"An array of objects, one for each condition that determines which jobs to exclude from the results.\"\n        }\n      ]\n    },\n    \"includes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfListJobsFilterTerm\"\n        },\n        {\n          \"description\": \"An array of objects, one for each condition that determines which\
  \ jobs to include in the results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-list-jobs-filter-criteria-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ListJobsFilterCriteria
---
