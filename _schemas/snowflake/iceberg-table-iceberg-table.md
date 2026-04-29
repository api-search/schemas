---
description: A Snowflake iceberg table
layout: schema
name: IcebergTable
properties_list:
- description: Name of the iceberg table
  name: name
  type: string
- description: user comment associated to an object in the dictionary
  name: comment
  type: string
- description: True if change tracking is enabled, allowing streams and CHANGES to be used on the entity.
  name: change_tracking
  type: boolean
- description: Maximum number of days to extend data retention beyond the retention period to prevent a stream becoming stale.
  name: max_data_extension_time_in_days
  type: integer
- description: Name of an external volume that will be used for persisted Iceberg metadata and data files.
  name: external_volume
  type: string
- description: number of days to retain the old version of deleted/updated data
  name: data_retention_time_in_days
  type: integer
- description: Name of the catalog integration to sync this table
  name: catalog_sync
  type: string
- description: Name of the catalog integration to use for iceberg tables
  name: catalog
  type: string
- description: Storage serialization policy used for managed Iceberg table. This include encodings and compressions
  name: storage_serialization_policy
  type: string
- description: Date and time when the iceberg table was created.
  name: created_on
  type: string
- description: Database in which the iceberg table is stored
  name: database_name
  type: string
- description: Schema in which the iceberg table is stored
  name: schema_name
  type: string
- description: Role that owns the iceberg table
  name: owner
  type: string
- description: The type of role that owns the iceberg table
  name: owner_role_type
  type: string
- description: Type of Iceberg table. UNMANAGED if the table is not managed by Snowflake. NOT ICEBERG otherwise.
  name: iceberg_table_type
  type: string
- description: Name of the table as recognized by the catalog.
  name: catalog_table_name
  type: string
- description: Catalog namespace for the table. The namespace defined when the table was created. Otherwise, the default namespace associated with the catalog integration used by the table. If you’re syncing the tab
  name: catalog_namespace
  type: string
- description: Signifies whether Snowflake can write metadata to the location specified by the file_path.
  name: can_write_metadata
  type: string
- description: Specifies one or more columns or column expressions in the table as the clustering key.
  name: cluster_by
  type: array
- description: ''
  name: columns
  type: array
- description: The path to a directory where Snowflake can write data and metadata files for the table.
  name: base_location
  type: string
- description: Specifies whether to replace invalid characters in the column names
  name: replace_invalid_characters
  type: boolean
- description: Specifies whether to automatically refresh the table metadata
  name: auto_refresh
  type: boolean
- description: Specifies the relative path of the Iceberg metadata file to use for column definitions.
  name: metadata_file_path
  type: string
- description: ''
  name: constraints
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/iceberg-table-iceberg-table-schema.json
slug: iceberg-table-iceberg-table
source_filename: iceberg-table-iceberg-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IcebergTable\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake iceberg table\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the iceberg table\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"user comment associated to an object in the dictionary\"\n    },\n    \"change_tracking\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if change tracking is enabled, allowing streams and CHANGES to be used on the entity.\"\n    },\n    \"max_data_extension_time_in_days\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of days to extend data retention beyond the retention period to prevent a stream becoming stale.\"\n    },\n    \"external_volume\": {\n      \"type\": \"string\",\n      \"description\": \"Name of an external volume that will be used for persisted\
  \ Iceberg metadata and data files.\"\n    },\n    \"data_retention_time_in_days\": {\n      \"type\": \"integer\",\n      \"description\": \"number of days to retain the old version of deleted/updated data\"\n    },\n    \"catalog_sync\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the catalog integration to sync this table\"\n    },\n    \"catalog\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the catalog integration to use for iceberg tables\"\n    },\n    \"storage_serialization_policy\": {\n      \"type\": \"string\",\n      \"description\": \"Storage serialization policy used for managed Iceberg table. This include encodings and compressions\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the iceberg table was created.\"\n    },\n    \"database_name\": {\n      \"type\": \"string\",\n      \"description\": \"Database in which the iceberg table is stored\"\n    },\n    \"schema_name\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Schema in which the iceberg table is stored\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Role that owns the iceberg table\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the iceberg table\"\n    },\n    \"iceberg_table_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of Iceberg table. UNMANAGED if the table is not managed by Snowflake. NOT ICEBERG otherwise.\"\n    },\n    \"catalog_table_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the table as recognized by the catalog.\"\n    },\n    \"catalog_namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Catalog namespace for the table. The namespace defined when the table was created. Otherwise, the default namespace associated with the catalog integration used by the table. If you\\u2019re syncing the table to\
  \ Snowflake Open Catalog, the default is null.\"\n    },\n    \"can_write_metadata\": {\n      \"type\": \"string\",\n      \"description\": \"Signifies whether Snowflake can write metadata to the location specified by the file_path.\"\n    },\n    \"cluster_by\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies one or more columns or column expressions in the table as the clustering key.\"\n    },\n    \"columns\": {\n      \"type\": \"array\"\n    },\n    \"base_location\": {\n      \"type\": \"string\",\n      \"description\": \"The path to a directory where Snowflake can write data and metadata files for the table.\"\n    },\n    \"replace_invalid_characters\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether to replace invalid characters in the column names\"\n    },\n    \"auto_refresh\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether to automatically refresh the table metadata\"\n    },\n    \"metadata_file_path\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Specifies the relative path of the Iceberg metadata file to use for column definitions.\"\n    },\n    \"constraints\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/iceberg-table-iceberg-table-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: IcebergTable
---
