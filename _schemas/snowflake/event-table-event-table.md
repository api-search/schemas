---
description: A Snowflake event table
layout: schema
name: EventTable
properties_list:
- description: Name of the event table
  name: name
  type: string
- description: Cluster key column(s) or expression
  name: cluster_by
  type: array
- description: number of days to retain the old version of deleted/updated data
  name: data_retention_time_in_days
  type: integer
- description: Maximum number of days to extend data retention beyond the retention period to prevent a stream becoming stale.
  name: max_data_extension_time_in_days
  type: integer
- description: True if change tracking is enabled, allowing streams and CHANGES to be used on the entity.
  name: change_tracking
  type: boolean
- description: Collation that is used for all the new columns created by the DDL statements (if not specified)
  name: default_ddl_collation
  type: string
- description: user comment associated to an object in the dictionary
  name: comment
  type: string
- description: Date and time when the event table was created.
  name: created_on
  type: string
- description: Database in which the event table is stored
  name: database_name
  type: string
- description: Schema in which the event table is stored
  name: schema_name
  type: string
- description: Role that owns the event table
  name: owner
  type: string
- description: The type of role that owns the event table
  name: owner_role_type
  type: string
- description: Number of rows in the table.
  name: rows
  type: integer
- description: Number of bytes that will be scanned if the entire table is scanned in a query.Note that this number may be different than the number of actual physical bytes stored on-disk for the table
  name: bytes
  type: integer
- description: If Automatic Clustering is enabled for your account, specifies whether it is explicitly enabled or disabled for the table.
  name: automatic_clustering
  type: boolean
- description: If ON, the table has the search optimization service enabled
  name: search_optimization
  type: boolean
- description: Percentage of the table that has been optimized for search
  name: search_optimization_progress
  type: integer
- description: Number of additional bytes of storage that the search optimization service consumes for this table
  name: search_optimization_bytes
  type: integer
- description: ''
  name: columns
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/event-table-event-table-schema.json
slug: event-table-event-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventTable\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake event table\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the event table\"\n    },\n    \"cluster_by\": {\n      \"type\": \"array\",\n      \"description\": \"Cluster key column(s) or expression\"\n    },\n    \"data_retention_time_in_days\": {\n      \"type\": \"integer\",\n      \"description\": \"number of days to retain the old version of deleted/updated data\"\n    },\n    \"max_data_extension_time_in_days\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of days to extend data retention beyond the retention period to prevent a stream becoming stale.\"\n    },\n    \"change_tracking\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if change tracking is enabled, allowing streams and CHANGES to be used on the entity.\"\
  \n    },\n    \"default_ddl_collation\": {\n      \"type\": \"string\",\n      \"description\": \"Collation that is used for all the new columns created by the DDL statements (if not specified)\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"user comment associated to an object in the dictionary\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the event table was created.\"\n    },\n    \"database_name\": {\n      \"type\": \"string\",\n      \"description\": \"Database in which the event table is stored\"\n    },\n    \"schema_name\": {\n      \"type\": \"string\",\n      \"description\": \"Schema in which the event table is stored\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Role that owns the event table\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the event table\"\n    },\n  \
  \  \"rows\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows in the table.\"\n    },\n    \"bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of bytes that will be scanned if the entire table is scanned in a query.Note that this number may be different than the number of actual physical bytes stored on-disk for the table\"\n    },\n    \"automatic_clustering\": {\n      \"type\": \"boolean\",\n      \"description\": \"If Automatic Clustering is enabled for your account, specifies whether it is explicitly enabled or disabled for the table.\"\n    },\n    \"search_optimization\": {\n      \"type\": \"boolean\",\n      \"description\": \"If ON, the table has the search optimization service enabled\"\n    },\n    \"search_optimization_progress\": {\n      \"type\": \"integer\",\n      \"description\": \"Percentage of the table that has been optimized for search\"\n    },\n    \"search_optimization_bytes\": {\n      \"type\": \"integer\",\n \
  \     \"description\": \"Number of additional bytes of storage that the search optimization service consumes for this table\"\n    },\n    \"columns\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/event-table-event-table-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: EventTable
---
