---
description: GetUnfilteredTableMetadataRequest schema from Amazon Glue API
layout: schema
name: GetUnfilteredTableMetadataRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: AuditContext
  type: object
- description: ''
  name: SupportedPermissionTypes
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-unfiltered-table-metadata-request-schema.json
slug: glue-get-unfiltered-table-metadata-request
source_filename: glue-get-unfiltered-table-metadata-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-unfiltered-table-metadata-request-schema.json\",\n  \"title\": \"GetUnfilteredTableMetadataRequest\",\n  \"description\": \"GetUnfilteredTableMetadataRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The catalog ID where the table resides.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"(Required) Specifies the name of a database that contains the table.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"(Required) Specifies the name of a table for which you are requesting metadata.\"\n        }\n      ]\n    },\n    \"AuditContext\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditContext\"\n        },\n        {\n          \"description\": \"A structure containing Lake Formation audit context information.\"\n        }\n      ]\n    },\n    \"SupportedPermissionTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionTypeList\"\n        },\n        {\n          \"description\": \"(Required) A list of supported permission types. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CatalogId\",\n    \"DatabaseName\",\n    \"Name\",\n    \"SupportedPermissionTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-unfiltered-table-metadata-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetUnfilteredTableMetadataRequest
---
