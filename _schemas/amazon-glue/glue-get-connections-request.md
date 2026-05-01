---
description: GetConnectionsRequest schema from Amazon Glue API
layout: schema
name: GetConnectionsRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: Filter
  type: object
- description: ''
  name: HidePassword
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-connections-request-schema.json
slug: glue-get-connections-request
source_filename: glue-get-connections-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-connections-request-schema.json\",\n  \"title\": \"GetConnectionsRequest\",\n  \"description\": \"GetConnectionsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog in which the connections reside. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"Filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetConnectionsFilter\"\n        },\n        {\n          \"description\": \"A filter that controls which connections are returned.\"\n        }\n      ]\n    },\n    \"HidePassword\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Allows you to retrieve the connection metadata without returning the password. For instance, the Glue console uses this flag to retrieve the connection, and does not display the password. Set this parameter when the caller might not have permission to use the KMS key to decrypt the password, but it does have permission to access the rest of the connection properties.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, if this is a continuation call.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum number of connections to return in one response.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-connections-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetConnectionsRequest
---
