---
description: GetWorkflowRunsRequest schema from Amazon Glue API
layout: schema
name: GetWorkflowRunsRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: IncludeGraph
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-workflow-runs-request-schema.json
slug: glue-get-workflow-runs-request
source_filename: glue-get-workflow-runs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-runs-request-schema.json\",\n  \"title\": \"GetWorkflowRunsRequest\",\n  \"description\": \"GetWorkflowRunsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Name of the workflow whose metadata of runs should be returned.\"\n        }\n      ]\n    },\n    \"IncludeGraph\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Specifies whether to include the workflow graph in response or not.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\
  \n        },\n        {\n          \"description\": \"The maximum size of the response.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum number of workflow runs to be included in the response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-workflow-runs-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetWorkflowRunsRequest
---
