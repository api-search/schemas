---
description: ResumeWorkflowRunResponse schema from Amazon Glue API
layout: schema
name: ResumeWorkflowRunResponse
properties_list:
- description: ''
  name: RunId
  type: object
- description: ''
  name: NodeIds
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-resume-workflow-run-response-schema.json
slug: glue-resume-workflow-run-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-resume-workflow-run-response-schema.json\",\n  \"title\": \"ResumeWorkflowRunResponse\",\n  \"description\": \"ResumeWorkflowRunResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdString\"\n        },\n        {\n          \"description\": \"The new ID assigned to the resumed workflow run. Each resume of a workflow run will have a new run ID.\"\n        }\n      ]\n    },\n    \"NodeIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeIdList\"\n        },\n        {\n          \"description\": \"A list of the node IDs for the nodes that were actually restarted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-resume-workflow-run-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ResumeWorkflowRunResponse
---
