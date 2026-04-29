---
description: UpdateDatabaseRequest schema from Amazon Glue API
layout: schema
name: UpdateDatabaseRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: DatabaseInput
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-database-request-schema.json
slug: glue-update-database-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-database-request-schema.json\",\n  \"title\": \"UpdateDatabaseRequest\",\n  \"description\": \"UpdateDatabaseRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog in which the metadata database resides. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the database to update in the catalog. For Hive compatibility, this is folded to lowercase.\"\n    \
  \    }\n      ]\n    },\n    \"DatabaseInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseInput\"\n        },\n        {\n          \"description\": \"A <code>DatabaseInput</code> object specifying the new definition of the metadata database in the catalog.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"DatabaseInput\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-database-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateDatabaseRequest
---
