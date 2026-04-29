---
description: GetDataflowGraphResponse schema from Amazon Glue API
layout: schema
name: GetDataflowGraphResponse
properties_list:
- description: ''
  name: DagNodes
  type: object
- description: ''
  name: DagEdges
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-dataflow-graph-response-schema.json
slug: glue-get-dataflow-graph-response
source_filename: glue-get-dataflow-graph-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-dataflow-graph-response-schema.json\",\n  \"title\": \"GetDataflowGraphResponse\",\n  \"description\": \"GetDataflowGraphResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DagNodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DagNodes\"\n        },\n        {\n          \"description\": \"A list of the nodes in the resulting DAG.\"\n        }\n      ]\n    },\n    \"DagEdges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DagEdges\"\n        },\n        {\n          \"description\": \"A list of the edges in the resulting DAG.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-dataflow-graph-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDataflowGraphResponse
---
