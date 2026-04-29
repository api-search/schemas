---
description: BatchGetDevEndpointsResponse schema from Amazon Glue API
layout: schema
name: BatchGetDevEndpointsResponse
properties_list:
- description: ''
  name: DevEndpoints
  type: object
- description: ''
  name: DevEndpointsNotFound
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-dev-endpoints-response-schema.json
slug: glue-batch-get-dev-endpoints-response
source_filename: glue-batch-get-dev-endpoints-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-dev-endpoints-response-schema.json\",\n  \"title\": \"BatchGetDevEndpointsResponse\",\n  \"description\": \"BatchGetDevEndpointsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DevEndpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEndpointList\"\n        },\n        {\n          \"description\": \"A list of <code>DevEndpoint</code> definitions.\"\n        }\n      ]\n    },\n    \"DevEndpointsNotFound\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEndpointNames\"\n        },\n        {\n          \"description\": \"A list of <code>DevEndpoints</code> not found.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-dev-endpoints-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetDevEndpointsResponse
---
