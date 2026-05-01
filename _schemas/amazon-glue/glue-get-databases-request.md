---
description: GetDatabasesRequest schema from Amazon Glue API
layout: schema
name: GetDatabasesRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: ResourceShareType
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-databases-request-schema.json
slug: glue-get-databases-request
source_filename: glue-get-databases-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-databases-request-schema.json\",\n  \"title\": \"GetDatabasesRequest\",\n  \"description\": \"GetDatabasesRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog from which to retrieve <code>Databases</code>. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, if this is a continuation call.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogGetterPageSize\"\n        },\n        {\n          \"description\": \"The maximum number of databases to return in one response.\"\n        }\n      ]\n    },\n    \"ResourceShareType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceShareType\"\n        },\n        {\n          \"description\": \"<p>Allows you to specify that you want to list the databases shared with your account. The allowable values are <code>FEDERATED</code>, <code>FOREIGN</code> or <code>ALL</code>. </p> <ul> <li> <p>If set to <code>FEDERATED</code>, will list the federated databases (referencing an external entity) shared with your account.</p> </li> <li> <p>If set to <code>FOREIGN</code>, will list the databases shared with your account. </p> </li> <li> <p>If set to <code>ALL</code>, will list the databases shared with your account, as well as the databases in yor local account. </p> </li> </ul>\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-databases-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDatabasesRequest
---
