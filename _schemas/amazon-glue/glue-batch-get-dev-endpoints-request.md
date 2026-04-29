---
description: BatchGetDevEndpointsRequest schema from Amazon Glue API
layout: schema
name: BatchGetDevEndpointsRequest
properties_list:
- description: ''
  name: DevEndpointNames
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-dev-endpoints-request-schema.json
slug: glue-batch-get-dev-endpoints-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-dev-endpoints-request-schema.json\",\n  \"title\": \"BatchGetDevEndpointsRequest\",\n  \"description\": \"BatchGetDevEndpointsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DevEndpointNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEndpointNames\"\n        },\n        {\n          \"description\": \"The list of <code>DevEndpoint</code> names, which might be the names returned from the <code>ListDevEndpoint</code> operation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DevEndpointNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-dev-endpoints-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetDevEndpointsRequest
---
