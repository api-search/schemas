---
description: CreateWorkflowRequest schema from Amazon Glue API
layout: schema
name: CreateWorkflowRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: DefaultRunProperties
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: MaxConcurrentRuns
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-workflow-request-schema.json
slug: glue-create-workflow-request
source_filename: glue-create-workflow-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-workflow-request-schema.json\",\n  \"title\": \"CreateWorkflowRequest\",\n  \"description\": \"CreateWorkflowRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name to be assigned to the workflow. It should be unique within your account.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A description of the workflow.\"\n        }\n      ]\n    },\n    \"DefaultRunProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRunProperties\"\
  \n        },\n        {\n          \"description\": \"A collection of properties to be used as part of each execution of the workflow.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"The tags to be used with this workflow.\"\n        }\n      ]\n    },\n    \"MaxConcurrentRuns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"You can use this parameter to prevent unwanted multiple updates to data, to control costs, or in some cases, to prevent exceeding the maximum number of concurrent runs of any of the component jobs. If you leave this parameter blank, there is no limit to the number of concurrent workflow runs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-workflow-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateWorkflowRequest
---
