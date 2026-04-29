---
description: A Snowflake table
layout: schema
name: Table
properties_list:
- description: Specifies the name for the table, must be unique for the schema in which the table is created
  name: name
  type: string
- description: Table type - permanent, transient, or temporary
  name: kind
  type: string
- description: Specifies one or more columns or column expressions in the table as the clustering key
  name: cluster_by
  type: array
- description: Table has schema evolution enabled or disabled
  name: enable_schema_evolution
  type: boolean
- description: Change tracking is enabled or disabled
  name: change_tracking
  type: boolean
- description: Specifies the retention period for the table so that Time Travel actions SELECT, CLONE, UNDROP can be performed on historical data in the table
  name: data_retention_time_in_days
  type: integer
- description: Specifies the retention period for the table so that Time Travel actions SELECT, CLONE, UNDROP can be performed on historical data in the table
  name: max_data_extension_time_in_days
  type: integer
- description: Specifies a default collation specification for the columns in the table, including columns added to the table in the future
  name: default_ddl_collation
  type: string
- description: ''
  name: columns
  type: array
- description: ''
  name: constraints
  type: array
- description: Comment for the table
  name: comment
  type: string
- description: Date and time when the table was created.
  name: created_on
  type: string
- description: Database in which the table is stored
  name: database_name
  type: string
- description: Schema in which the table is stored
  name: schema_name
  type: string
- description: Number of rows in the table. Returns NULL for external tables.
  name: rows
  type: integer
- description: Number of bytes that will be scanned if the entire table is scanned in a query. Note that this number may be different than the number of actual physical bytes stored on-disk for the table
  name: bytes
  type: integer
- description: Role that owns the table
  name: owner
  type: string
- description: Date and time when the table was dropped
  name: dropped_on
  type: string
- description: If Automatic Clustering is enabled for your account, specifies whether it is explicitly enabled or disabled for the table.
  name: automatic_clustering
  type: boolean
- description: If ON, the table has the search optimization service enabled
  name: search_optimization
  type: boolean
- description: Percentage of the table that has been optimized for search.
  name: search_optimization_progress
  type: integer
- description: Number of additional bytes of storage that the search optimization service consumes for this table
  name: search_optimization_bytes
  type: integer
- description: The type of role that owns the object.
  name: owner_role_type
  type: string
- description: Name of the budget if the object is monitored by a budget
  name: budget
  type: string
- description: Type of the table
  name: table_type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/table-table-schema.json
slug: table-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Table\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake table\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the name for the table, must be unique for the schema in which the table is created\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Table type - permanent, transient, or temporary\"\n    },\n    \"cluster_by\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies one or more columns or column expressions in the table as the clustering key\"\n    },\n    \"enable_schema_evolution\": {\n      \"type\": \"boolean\",\n      \"description\": \"Table has schema evolution enabled or disabled\"\n    },\n    \"change_tracking\": {\n      \"type\": \"boolean\",\n      \"description\": \"Change tracking is enabled or disabled\"\n    },\n    \"data_retention_time_in_days\": {\n  \
  \    \"type\": \"integer\",\n      \"description\": \"Specifies the retention period for the table so that Time Travel actions SELECT, CLONE, UNDROP can be performed on historical data in the table\"\n    },\n    \"max_data_extension_time_in_days\": {\n      \"type\": \"integer\",\n      \"description\": \"Specifies the retention period for the table so that Time Travel actions SELECT, CLONE, UNDROP can be performed on historical data in the table\"\n    },\n    \"default_ddl_collation\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies a default collation specification for the columns in the table, including columns added to the table in the future\"\n    },\n    \"columns\": {\n      \"type\": \"array\"\n    },\n    \"constraints\": {\n      \"type\": \"array\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Comment for the table\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when\
  \ the table was created.\"\n    },\n    \"database_name\": {\n      \"type\": \"string\",\n      \"description\": \"Database in which the table is stored\"\n    },\n    \"schema_name\": {\n      \"type\": \"string\",\n      \"description\": \"Schema in which the table is stored\"\n    },\n    \"rows\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows in the table. Returns NULL for external tables.\"\n    },\n    \"bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of bytes that will be scanned if the entire table is scanned in a query. Note that this number may be different than the number of actual physical bytes stored on-disk for the table\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Role that owns the table\"\n    },\n    \"dropped_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the table was dropped\"\n    },\n    \"automatic_clustering\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"If Automatic Clustering is enabled for your account, specifies whether it is explicitly enabled or disabled for the table.\"\n    },\n    \"search_optimization\": {\n      \"type\": \"boolean\",\n      \"description\": \"If ON, the table has the search optimization service enabled\"\n    },\n    \"search_optimization_progress\": {\n      \"type\": \"integer\",\n      \"description\": \"Percentage of the table that has been optimized for search.\"\n    },\n    \"search_optimization_bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of additional bytes of storage that the search optimization service consumes for this table\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the object.\"\n    },\n    \"budget\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the budget if the object is monitored by a budget\"\n    },\n    \"table_type\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Type of the table\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/table-table-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Table
---
