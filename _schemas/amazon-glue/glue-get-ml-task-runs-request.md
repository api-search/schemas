---
description: GetMLTaskRunsRequest schema from Amazon Glue API
layout: schema
name: GetMLTaskRunsRequest
properties_list:
- description: ''
  name: TransformId
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: Filter
  type: object
- description: ''
  name: Sort
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-ml-task-runs-request-schema.json
slug: glue-get-ml-task-runs-request
source_filename: glue-get-ml-task-runs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-ml-task-runs-request-schema.json\",\n  \"title\": \"GetMLTaskRunsRequest\",\n  \"description\": \"GetMLTaskRunsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransformId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique identifier of the machine learning transform.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A token for pagination of the results. The default is empty.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\
  \n        },\n        {\n          \"description\": \"The maximum number of results to return. \"\n        }\n      ]\n    },\n    \"Filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskRunFilterCriteria\"\n        },\n        {\n          \"description\": \"The filter criteria, in the <code>TaskRunFilterCriteria</code> structure, for the task run.\"\n        }\n      ]\n    },\n    \"Sort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskRunSortCriteria\"\n        },\n        {\n          \"description\": \"The sorting criteria, in the <code>TaskRunSortCriteria</code> structure, for the task run.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TransformId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-ml-task-runs-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetMLTaskRunsRequest
---
