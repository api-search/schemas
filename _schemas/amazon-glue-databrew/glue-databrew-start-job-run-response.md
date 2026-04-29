---
description: StartJobRunResponse schema from Amazon Glue DataBrew API
layout: schema
name: StartJobRunResponse
properties_list:
- description: ''
  name: RunId
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-start-job-run-response-schema.json
slug: glue-databrew-start-job-run-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-start-job-run-response-schema.json\",\n  \"title\": \"StartJobRunResponse\",\n  \"description\": \"StartJobRunResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobRunId\"\n        },\n        {\n          \"description\": \"A system-generated identifier for this particular job run.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RunId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-start-job-run-response-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: StartJobRunResponse
---
