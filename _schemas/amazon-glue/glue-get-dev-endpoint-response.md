---
description: GetDevEndpointResponse schema from Amazon Glue API
layout: schema
name: GetDevEndpointResponse
properties_list:
- description: ''
  name: DevEndpoint
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-dev-endpoint-response-schema.json
slug: glue-get-dev-endpoint-response
source_filename: glue-get-dev-endpoint-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-dev-endpoint-response-schema.json\",\n  \"title\": \"GetDevEndpointResponse\",\n  \"description\": \"GetDevEndpointResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DevEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEndpoint\"\n        },\n        {\n          \"description\": \"A <code>DevEndpoint</code> definition.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-dev-endpoint-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDevEndpointResponse
---
