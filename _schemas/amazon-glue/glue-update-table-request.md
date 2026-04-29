---
description: UpdateTableRequest schema from Amazon Glue API
layout: schema
name: UpdateTableRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: TableInput
  type: object
- description: ''
  name: SkipArchive
  type: object
- description: ''
  name: TransactionId
  type: object
- description: ''
  name: VersionId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-table-request-schema.json
slug: glue-update-table-request
source_filename: glue-update-table-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-table-request-schema.json\",\n  \"title\": \"UpdateTableRequest\",\n  \"description\": \"UpdateTableRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog where the table resides. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the catalog database in which the table resides. For Hive compatibility, this name is entirely lowercase.\"\n      \
  \  }\n      ]\n    },\n    \"TableInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TableInput\"\n        },\n        {\n          \"description\": \"An updated <code>TableInput</code> object to define the metadata table in the catalog.\"\n        }\n      ]\n    },\n    \"SkipArchive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanNullable\"\n        },\n        {\n          \"description\": \"By default, <code>UpdateTable</code> always creates an archived version of the table before updating it. However, if <code>skipArchive</code> is set to true, <code>UpdateTable</code> does not create the archived version.\"\n        }\n      ]\n    },\n    \"TransactionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransactionIdString\"\n        },\n        {\n          \"description\": \"The transaction ID at which to update the table contents. \"\n        }\n      ]\n    },\n    \"VersionId\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionString\"\n        },\n        {\n          \"description\": \"The version ID at which to update the table contents. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseName\",\n    \"TableInput\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-table-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateTableRequest
---
