---
description: ListDevEndpointsResponse schema from Amazon Glue API
layout: schema
name: ListDevEndpointsResponse
properties_list:
- description: ''
  name: DevEndpointNames
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-dev-endpoints-response-schema.json
slug: glue-list-dev-endpoints-response
source_filename: glue-list-dev-endpoints-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-dev-endpoints-response-schema.json\",\n  \"title\": \"ListDevEndpointsResponse\",\n  \"description\": \"ListDevEndpointsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DevEndpointNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEndpointNameList\"\n        },\n        {\n          \"description\": \"The names of all the <code>DevEndpoint</code>s in the account, or the <code>DevEndpoint</code>s with the specified tags.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A continuation token, if the returned list does not contain the last metric available.\"\n        }\n   \
  \   ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-dev-endpoints-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListDevEndpointsResponse
---
