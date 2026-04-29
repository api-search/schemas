---
description: DeleteDevEndpointRequest schema from Amazon Glue API
layout: schema
name: DeleteDevEndpointRequest
properties_list:
- description: ''
  name: EndpointName
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-dev-endpoint-request-schema.json
slug: glue-delete-dev-endpoint-request
source_filename: glue-delete-dev-endpoint-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-dev-endpoint-request-schema.json\",\n  \"title\": \"DeleteDevEndpointRequest\",\n  \"description\": \"DeleteDevEndpointRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The name of the <code>DevEndpoint</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-dev-endpoint-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteDevEndpointRequest
---
