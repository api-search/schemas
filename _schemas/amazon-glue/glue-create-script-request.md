---
description: CreateScriptRequest schema from Amazon Glue API
layout: schema
name: CreateScriptRequest
properties_list:
- description: ''
  name: DagNodes
  type: object
- description: ''
  name: DagEdges
  type: object
- description: ''
  name: Language
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-script-request-schema.json
slug: glue-create-script-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-script-request-schema.json\",\n  \"title\": \"CreateScriptRequest\",\n  \"description\": \"CreateScriptRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DagNodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DagNodes\"\n        },\n        {\n          \"description\": \"A list of the nodes in the DAG.\"\n        }\n      ]\n    },\n    \"DagEdges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DagEdges\"\n        },\n        {\n          \"description\": \"A list of the edges in the DAG.\"\n        }\n      ]\n    },\n    \"Language\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Language\"\n        },\n        {\n          \"description\": \"The programming\
  \ language of the resulting code from the DAG.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-script-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateScriptRequest
---
