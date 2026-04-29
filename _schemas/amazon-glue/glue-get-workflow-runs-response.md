---
description: GetWorkflowRunsResponse schema from Amazon Glue API
layout: schema
name: GetWorkflowRunsResponse
properties_list:
- description: ''
  name: Runs
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-workflow-runs-response-schema.json
slug: glue-get-workflow-runs-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-runs-response-schema.json\",\n  \"title\": \"GetWorkflowRunsResponse\",\n  \"description\": \"GetWorkflowRunsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Runs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRuns\"\n        },\n        {\n          \"description\": \"A list of workflow run metadata objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A continuation token, if not all requested workflow runs have been returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-runs-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetWorkflowRunsResponse
---
