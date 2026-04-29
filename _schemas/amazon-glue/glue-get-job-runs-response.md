---
description: GetJobRunsResponse schema from Amazon Glue API
layout: schema
name: GetJobRunsResponse
properties_list:
- description: ''
  name: JobRuns
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-job-runs-response-schema.json
slug: glue-get-job-runs-response
source_filename: glue-get-job-runs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-job-runs-response-schema.json\",\n  \"title\": \"GetJobRunsResponse\",\n  \"description\": \"GetJobRunsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobRuns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobRunList\"\n        },\n        {\n          \"description\": \"A list of job-run metadata objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A continuation token, if not all requested job runs have been returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-job-runs-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetJobRunsResponse
---
