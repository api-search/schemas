---
description: ResumeWorkflowRunRequest schema from Amazon Glue API
layout: schema
name: ResumeWorkflowRunRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: RunId
  type: object
- description: ''
  name: NodeIds
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-resume-workflow-run-request-schema.json
slug: glue-resume-workflow-run-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-resume-workflow-run-request-schema.json\",\n  \"title\": \"ResumeWorkflowRunRequest\",\n  \"description\": \"ResumeWorkflowRunRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the workflow to resume.\"\n        }\n      ]\n    },\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdString\"\n        },\n        {\n          \"description\": \"The ID of the workflow run to resume.\"\n        }\n      ]\n    },\n    \"NodeIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeIdList\"\n        },\n        {\n          \"description\"\
  : \"A list of the node IDs for the nodes you want to restart. The nodes that are to be restarted must have a run attempt in the original run.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"RunId\",\n    \"NodeIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-resume-workflow-run-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ResumeWorkflowRunRequest
---
