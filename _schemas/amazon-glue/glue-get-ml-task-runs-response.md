---
description: GetMLTaskRunsResponse schema from Amazon Glue API
layout: schema
name: GetMLTaskRunsResponse
properties_list:
- description: ''
  name: TaskRuns
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-ml-task-runs-response-schema.json
slug: glue-get-ml-task-runs-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-ml-task-runs-response-schema.json\",\n  \"title\": \"GetMLTaskRunsResponse\",\n  \"description\": \"GetMLTaskRunsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TaskRuns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskRunList\"\n        },\n        {\n          \"description\": \"A list of task runs that are associated with the transform.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A pagination token, if more results are available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-ml-task-runs-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetMLTaskRunsResponse
---
