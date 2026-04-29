---
description: BatchStopJobRunRequest schema from Amazon Glue API
layout: schema
name: BatchStopJobRunRequest
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: JobRunIds
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-stop-job-run-request-schema.json
slug: glue-batch-stop-job-run-request
source_filename: glue-batch-stop-job-run-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-stop-job-run-request-schema.json\",\n  \"title\": \"BatchStopJobRunRequest\",\n  \"description\": \"BatchStopJobRunRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the job definition for which to stop job runs.\"\n        }\n      ]\n    },\n    \"JobRunIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchStopJobRunJobRunIdList\"\n        },\n        {\n          \"description\": \"A list of the <code>JobRunIds</code> that should be stopped for that job definition.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobName\",\n    \"JobRunIds\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-stop-job-run-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchStopJobRunRequest
---
