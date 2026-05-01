---
description: GetUnfilteredTableMetadataResponse schema from Amazon Glue API
layout: schema
name: GetUnfilteredTableMetadataResponse
properties_list:
- description: ''
  name: Table
  type: object
- description: ''
  name: AuthorizedColumns
  type: object
- description: ''
  name: IsRegisteredWithLakeFormation
  type: object
- description: ''
  name: CellFilters
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-unfiltered-table-metadata-response-schema.json
slug: glue-get-unfiltered-table-metadata-response
source_filename: glue-get-unfiltered-table-metadata-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-unfiltered-table-metadata-response-schema.json\",\n  \"title\": \"GetUnfilteredTableMetadataResponse\",\n  \"description\": \"GetUnfilteredTableMetadataResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Table\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Table\"\n        },\n        {\n          \"description\": \"A Table object containing the table metadata.\"\n        }\n      ]\n    },\n    \"AuthorizedColumns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameStringList\"\n        },\n        {\n          \"description\": \"A list of column names that the user has been granted access to.\"\n        }\n      ]\n    },\n    \"IsRegisteredWithLakeFormation\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that indicates whether the partition location is registered with Lake Formation.\"\n        }\n      ]\n    },\n    \"CellFilters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnRowFilterList\"\n        },\n        {\n          \"description\": \"A list of column row filters.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-unfiltered-table-metadata-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetUnfilteredTableMetadataResponse
---
