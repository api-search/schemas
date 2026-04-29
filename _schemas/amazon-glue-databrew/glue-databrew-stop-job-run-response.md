---
description: StopJobRunResponse schema from Amazon Glue DataBrew API
layout: schema
name: StopJobRunResponse
properties_list:
- description: ''
  name: RunId
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-stop-job-run-response-schema.json
slug: glue-databrew-stop-job-run-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-stop-job-run-response-schema.json\",\n  \"title\": \"StopJobRunResponse\",\n  \"description\": \"StopJobRunResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobRunId\"\n        },\n        {\n          \"description\": \"The ID of the job run that you stopped.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RunId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-stop-job-run-response-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: StopJobRunResponse
---
