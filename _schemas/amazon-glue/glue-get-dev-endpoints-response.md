---
description: GetDevEndpointsResponse schema from Amazon Glue API
layout: schema
name: GetDevEndpointsResponse
properties_list:
- description: ''
  name: DevEndpoints
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-dev-endpoints-response-schema.json
slug: glue-get-dev-endpoints-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-dev-endpoints-response-schema.json\",\n  \"title\": \"GetDevEndpointsResponse\",\n  \"description\": \"GetDevEndpointsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DevEndpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEndpointList\"\n        },\n        {\n          \"description\": \"A list of <code>DevEndpoint</code> definitions.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A continuation token, if not all <code>DevEndpoint</code> definitions have yet been returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-dev-endpoints-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDevEndpointsResponse
---
