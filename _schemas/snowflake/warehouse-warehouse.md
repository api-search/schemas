---
description: A Snowflake virtual warehouse
layout: schema
name: Warehouse
properties_list:
- description: 'Type of warehouse, possible types: STANDARD, SNOWPARK-OPTIMIZED'
  name: warehouse_type
  type: string
- description: 'Size of warehouse, possible sizes: XSMALL, SMALL, MEDIUM, LARGE, XLARGE, XXLARGE, XXXLARGE, X4LARGE, X5LARGE, X6LARGE'
  name: warehouse_size
  type: string
- description: When resizing a warehouse, you can use this parameter to block the return of the ALTER WAREHOUSE command until the resize has finished provisioning all its compute resources
  name: wait_for_completion
  type: string
- description: Specifies the maximum number of clusters for a multi-cluster warehouse
  name: max_cluster_count
  type: integer
- description: Specifies the minimum number of clusters for a multi-cluster warehouse
  name: min_cluster_count
  type: integer
- description: 'Scaling policy of warehouse, possible scaling policies: STANDARD, ECONOMY'
  name: scaling_policy
  type: string
- description: time in seconds before auto suspend
  name: auto_suspend
  type: integer
- description: Specifies whether to automatically resume a warehouse when a SQL statement is submitted to it
  name: auto_resume
  type: string
- description: Specifies whether the warehouse is created initially in the Suspended state
  name: initially_suspended
  type: string
- description: Specifies a comment for the warehouse
  name: comment
  type: string
- description: Specifies whether to enable the query acceleration service for queries that rely on this warehouse for compute resources
  name: enable_query_acceleration
  type: string
- description: Specifies the maximum scale factor for leasing compute resources for query acceleration. The scale factor is used as a multiplier based on warehouse size
  name: query_acceleration_max_scale_factor
  type: integer
- description: Object parameter that specifies the concurrency level for SQL statements executed by a warehouse cluster
  name: max_concurrency_level
  type: integer
- description: Object parameter that specifies the time, in seconds, a SQL statement can be queued on a warehouse before it is canceled by the system
  name: statement_queued_timeout_in_seconds
  type: integer
- description: Object parameter that specifies the time, in seconds, after which a running SQL statement is canceled by the system
  name: statement_timeout_in_seconds
  type: integer
- description: '[Deprecated] Type of warehouse, possible types: STANDARD, SNOWPARK-OPTIMIZED'
  name: type
  type: string
- description: '[Deprecated] names of size: X-Small, Small, Medium, Large, X-Large, 2X-Large, 3X-Large, 4X-Large, 5X-Large, 6X-Large'
  name: size
  type: string
- description: 'The state of warehouse, possible states: STARTED, STARTING, DYNAMIC, SUSPENDED, RESIZING, RESUMING, SUSPENDING'
  name: state
  type: string
- description: Number of clusters currently started.
  name: started_clusters
  type: integer
- description: Number of SQL statements that are being executed by the warehouse.
  name: running
  type: integer
- description: Number of SQL statements that are queued for the warehouse.
  name: queued
  type: integer
- description: Whether the warehouse is the default for the current user.
  name: is_default
  type: boolean
- description: Whether the warehouse is in use for the session. Only one warehouse can be in use at a time for a session. To specify or change the warehouse for a session, use the USE WAREHOUSE command.
  name: is_current
  type: boolean
- description: Percentage of the warehouse compute resources that are provisioned and available.
  name: available
  type: string
- description: Percentage of the warehouse compute resources that are in the process of provisioning.
  name: provisioning
  type: string
- description: Percentage of the warehouse compute resources that are executing SQL statements, but will be shut down once the queries complete.
  name: quiescing
  type: string
- description: Percentage of the warehouse compute resources that are in a state other than available, provisioning, or quiescing.
  name: other
  type: string
- description: Date and time when the warehouse was created.
  name: created_on
  type: string
- description: Date and time when the warehouse was last started or restarted.
  name: resumed_on
  type: string
- description: Date and time when the warehouse was last updated, which includes changing any of the properties of the warehouse or changing the state (STARTED, SUSPENDED, RESIZING) of the warehouse.
  name: updated_on
  type: string
- description: Role that owns the warehouse.
  name: owner
  type: string
- description: Comment representing budget for warehouse.
  name: budget
  type: string
- description: ''
  name: kind
  type: string
- description: The type of role that owns the object.
  name: owner_role_type
  type: string
- description: Credit limit that are can be executed by the warehouse.
  name: warehouse_credit_limit
  type: integer
- description: 'Names of size: X-Small, Small, Medium, Large, X-Large, 2X-Large, 3X-Large, 4X-Large, 5X-Large, 6X-Large'
  name: target_statement_size
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/warehouse-warehouse-schema.json
slug: warehouse-warehouse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Warehouse\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake virtual warehouse\",\n  \"properties\": {\n    \"warehouse_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of warehouse, possible types: STANDARD, SNOWPARK-OPTIMIZED\"\n    },\n    \"warehouse_size\": {\n      \"type\": \"string\",\n      \"description\": \"Size of warehouse, possible sizes: XSMALL, SMALL, MEDIUM, LARGE, XLARGE, XXLARGE, XXXLARGE, X4LARGE, X5LARGE, X6LARGE\"\n    },\n    \"wait_for_completion\": {\n      \"type\": \"string\",\n      \"description\": \"When resizing a warehouse, you can use this parameter to block the return of the ALTER WAREHOUSE command until the resize has finished provisioning all its compute resources\"\n    },\n    \"max_cluster_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Specifies the maximum number of clusters for a multi-cluster warehouse\"\
  \n    },\n    \"min_cluster_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Specifies the minimum number of clusters for a multi-cluster warehouse\"\n    },\n    \"scaling_policy\": {\n      \"type\": \"string\",\n      \"description\": \"Scaling policy of warehouse, possible scaling policies: STANDARD, ECONOMY\"\n    },\n    \"auto_suspend\": {\n      \"type\": \"integer\",\n      \"description\": \"time in seconds before auto suspend\"\n    },\n    \"auto_resume\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies whether to automatically resume a warehouse when a SQL statement is submitted to it\"\n    },\n    \"initially_suspended\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies whether the warehouse is created initially in the Suspended state\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies a comment for the warehouse\"\n    },\n    \"enable_query_acceleration\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Specifies whether to enable the query acceleration service for queries that rely on this warehouse for compute resources\"\n    },\n    \"query_acceleration_max_scale_factor\": {\n      \"type\": \"integer\",\n      \"description\": \"Specifies the maximum scale factor for leasing compute resources for query acceleration. The scale factor is used as a multiplier based on warehouse size\"\n    },\n    \"max_concurrency_level\": {\n      \"type\": \"integer\",\n      \"description\": \"Object parameter that specifies the concurrency level for SQL statements executed by a warehouse cluster\"\n    },\n    \"statement_queued_timeout_in_seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Object parameter that specifies the time, in seconds, a SQL statement can be queued on a warehouse before it is canceled by the system\"\n    },\n    \"statement_timeout_in_seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Object parameter\
  \ that specifies the time, in seconds, after which a running SQL statement  is canceled by the system\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"[Deprecated] Type of warehouse, possible types: STANDARD, SNOWPARK-OPTIMIZED\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"[Deprecated] names of size: X-Small, Small, Medium, Large, X-Large, 2X-Large, 3X-Large, 4X-Large, 5X-Large, 6X-Large\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state of warehouse, possible states: STARTED, STARTING, DYNAMIC, SUSPENDED, RESIZING, RESUMING, SUSPENDING\"\n    },\n    \"started_clusters\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of clusters currently started.\"\n    },\n    \"running\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of SQL statements that are being executed by the warehouse.\"\n    },\n    \"queued\": {\n      \"type\": \"integer\",\n\
  \      \"description\": \"Number of SQL statements that are queued for the warehouse.\"\n    },\n    \"is_default\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the warehouse is the default for the current user.\"\n    },\n    \"is_current\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the warehouse is in use for the session. Only one warehouse can be in use at a time for a session.  To specify or change the warehouse for a session, use the USE WAREHOUSE command.\"\n    },\n    \"available\": {\n      \"type\": \"string\",\n      \"description\": \"Percentage of the warehouse compute resources that are provisioned and available.\"\n    },\n    \"provisioning\": {\n      \"type\": \"string\",\n      \"description\": \"Percentage of the warehouse compute resources that are in the process of provisioning.\"\n    },\n    \"quiescing\": {\n      \"type\": \"string\",\n      \"description\": \"Percentage of the warehouse compute resources that are\
  \ executing SQL statements,  but will be shut down once the queries complete.\"\n    },\n    \"other\": {\n      \"type\": \"string\",\n      \"description\": \"Percentage of the warehouse compute resources that are in a state other than available,  provisioning, or quiescing.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the warehouse was created.\"\n    },\n    \"resumed_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the warehouse was last started or restarted.\"\n    },\n    \"updated_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the warehouse was last updated,  which includes changing any of the properties of the warehouse or changing the state (STARTED, SUSPENDED, RESIZING) of the warehouse.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Role that owns the warehouse.\"\n    },\n    \"budget\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Comment representing budget for warehouse.\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the object.\"\n    },\n    \"warehouse_credit_limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Credit limit that are can be executed by the warehouse.\"\n    },\n    \"target_statement_size\": {\n      \"type\": \"string\",\n      \"description\": \"Names of size: X-Small, Small, Medium, Large, X-Large, 2X-Large, 3X-Large, 4X-Large, 5X-Large, 6X-Large\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/warehouse-warehouse-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Warehouse
---
