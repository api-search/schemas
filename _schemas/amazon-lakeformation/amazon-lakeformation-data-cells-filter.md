---
description: A Lake Formation data cells filter for row-level and column-level security.
layout: schema
name: DataCellsFilter
properties_list:
- description: The ID of the Data Catalog.
  name: TableCatalogId
  type: string
- description: A database in the Data Catalog.
  name: DatabaseName
  type: string
- description: The name of the table.
  name: TableName
  type: string
- description: The name given by the user to the data filter cell.
  name: Name
  type: string
- description: A list of column names.
  name: ColumnNames
  type: array
- description: A PartiQL predicate for row-level filtering.
  name: RowFilter
  type: object
provider_name: AWS Lake Formation
provider_slug: amazon-lakeformation
schema_file: json-schema/amazon-lakeformation-data-cells-filter-schema.json
slug: amazon-lakeformation-data-cells-filter
source_filename: amazon-lakeformation-data-cells-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lakeformation/refs/heads/main/json-schema/amazon-lakeformation-data-cells-filter-schema.json\",\n  \"title\": \"DataCellsFilter\",\n  \"description\": \"A Lake Formation data cells filter for row-level and column-level security.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableCatalogId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Data Catalog.\"\n    },\n    \"DatabaseName\": {\n      \"type\": \"string\",\n      \"description\": \"A database in the Data Catalog.\"\n    },\n    \"TableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name given by the user to the data filter cell.\"\n    },\n    \"ColumnNames\": {\n      \"type\": \"array\",\n      \"description\": \"A list of\
  \ column names.\"\n    },\n    \"RowFilter\": {\n      \"type\": \"object\",\n      \"description\": \"A PartiQL predicate for row-level filtering.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lakeformation/refs/heads/main/json-schema/amazon-lakeformation-data-cells-filter-schema.json
tags:
- Analytics
- Data Lake
- Governance
title: DataCellsFilter
---
