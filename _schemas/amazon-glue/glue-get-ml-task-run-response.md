---
description: GetMLTaskRunResponse schema from Amazon Glue API
layout: schema
name: GetMLTaskRunResponse
properties_list:
- description: ''
  name: TransformId
  type: object
- description: ''
  name: TaskRunId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: LogGroupName
  type: object
- description: ''
  name: Properties
  type: object
- description: ''
  name: ErrorString
  type: object
- description: ''
  name: StartedOn
  type: object
- description: ''
  name: LastModifiedOn
  type: object
- description: ''
  name: CompletedOn
  type: object
- description: ''
  name: ExecutionTime
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-ml-task-run-response-schema.json
slug: glue-get-ml-task-run-response
source_filename: glue-get-ml-task-run-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-ml-task-run-response-schema.json\",\n  \"title\": \"GetMLTaskRunResponse\",\n  \"description\": \"GetMLTaskRunResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransformId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique identifier of the task run.\"\n        }\n      ]\n    },\n    \"TaskRunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique run identifier associated with this run.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskStatusType\"\n        },\n        {\n\
  \          \"description\": \"The status for this task run.\"\n        }\n      ]\n    },\n    \"LogGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The names of the log groups that are associated with the task run.\"\n        }\n      ]\n    },\n    \"Properties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskRunProperties\"\n        },\n        {\n          \"description\": \"The list of properties that are associated with the task run.\"\n        }\n      ]\n    },\n    \"ErrorString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The error strings that are associated with the task run.\"\n        }\n      ]\n    },\n    \"StartedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n   \
  \     {\n          \"description\": \"The date and time when this task run started.\"\n        }\n      ]\n    },\n    \"LastModifiedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when this task run was last modified.\"\n        }\n      ]\n    },\n    \"CompletedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when this task run was completed.\"\n        }\n      ]\n    },\n    \"ExecutionTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionTime\"\n        },\n        {\n          \"description\": \"The amount of time (in seconds) that the task run consumed resources.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-ml-task-run-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetMLTaskRunResponse
---
