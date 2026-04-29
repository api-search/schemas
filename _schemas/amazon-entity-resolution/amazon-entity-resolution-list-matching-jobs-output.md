---
description: ListMatchingJobsOutput schema from AWS EntityResolution
layout: schema
name: ListMatchingJobsOutput
properties_list:
- description: ''
  name: jobs
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-list-matching-jobs-output-schema.json
slug: amazon-entity-resolution-list-matching-jobs-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-list-matching-jobs-output-schema.json\",\n  \"title\": \"ListMatchingJobsOutput\",\n  \"description\": \"ListMatchingJobsOutput schema from AWS EntityResolution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobList\"\n        },\n        {\n          \"description\": \"A list of JobSummary objects, each of which contain the ID, status, start time, and end time of a job.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token from the previous <code>ListSchemaMappings</code> API call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-list-matching-jobs-output-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: ListMatchingJobsOutput
---
