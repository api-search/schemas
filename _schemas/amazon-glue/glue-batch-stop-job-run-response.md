---
description: BatchStopJobRunResponse schema from Amazon Glue API
layout: schema
name: BatchStopJobRunResponse
properties_list:
- description: ''
  name: SuccessfulSubmissions
  type: object
- description: ''
  name: Errors
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-stop-job-run-response-schema.json
slug: glue-batch-stop-job-run-response
source_filename: glue-batch-stop-job-run-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-stop-job-run-response-schema.json\",\n  \"title\": \"BatchStopJobRunResponse\",\n  \"description\": \"BatchStopJobRunResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SuccessfulSubmissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchStopJobRunSuccessfulSubmissionList\"\n        },\n        {\n          \"description\": \"A list of the JobRuns that were successfully submitted for stopping.\"\n        }\n      ]\n    },\n    \"Errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchStopJobRunErrorList\"\n        },\n        {\n          \"description\": \"A list of the errors that were encountered in trying to stop <code>JobRuns</code>, including the <code>JobRunId</code> for which\
  \ each error was encountered and details about the error.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-stop-job-run-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchStopJobRunResponse
---
