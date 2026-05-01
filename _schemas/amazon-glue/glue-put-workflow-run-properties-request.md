---
description: PutWorkflowRunPropertiesRequest schema from Amazon Glue API
layout: schema
name: PutWorkflowRunPropertiesRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: RunId
  type: object
- description: ''
  name: RunProperties
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-put-workflow-run-properties-request-schema.json
slug: glue-put-workflow-run-properties-request
source_filename: glue-put-workflow-run-properties-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-put-workflow-run-properties-request-schema.json\",\n  \"title\": \"PutWorkflowRunPropertiesRequest\",\n  \"description\": \"PutWorkflowRunPropertiesRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Name of the workflow which was run.\"\n        }\n      ]\n    },\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdString\"\n        },\n        {\n          \"description\": \"The ID of the workflow run for which the run properties should be updated.\"\n        }\n      ]\n    },\n    \"RunProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRunProperties\"\
  \n        },\n        {\n          \"description\": \"The properties to put for the specified run.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"RunId\",\n    \"RunProperties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-put-workflow-run-properties-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: PutWorkflowRunPropertiesRequest
---
