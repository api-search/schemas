---
description: GetDevEndpointRequest schema from Amazon Glue API
layout: schema
name: GetDevEndpointRequest
properties_list:
- description: ''
  name: EndpointName
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-dev-endpoint-request-schema.json
slug: glue-get-dev-endpoint-request
source_filename: glue-get-dev-endpoint-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-dev-endpoint-request-schema.json\",\n  \"title\": \"GetDevEndpointRequest\",\n  \"description\": \"GetDevEndpointRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"Name of the <code>DevEndpoint</code> to retrieve information for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-dev-endpoint-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDevEndpointRequest
---
