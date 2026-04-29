---
description: A Snowflake virtual warehouse provides the compute resources required to execute queries and perform DML operations. A warehouse can be started, suspended, resized, and configured for auto-suspend and auto-resume.
layout: schema
name: Snowflake Warehouse
properties_list:
- description: Identifier for the virtual warehouse. Must be unique within the account.
  name: name
  type: string
- description: Type of warehouse specifying the compute resource architecture.
  name: warehouse_type
  type: string
- description: Size of the warehouse determining the number of compute resources per cluster.
  name: warehouse_size
  type: string
- description: When resizing a warehouse, block the return of the ALTER WAREHOUSE command until the resize has finished provisioning all its compute resources.
  name: wait_for_completion
  type: string
- description: Specifies the maximum number of clusters for a multi-cluster warehouse. For a single-cluster warehouse, this value is 1.
  name: max_cluster_count
  type: integer
- description: Specifies the minimum number of clusters for a multi-cluster warehouse. For a single-cluster warehouse, this value is 1.
  name: min_cluster_count
  type: integer
- description: Scaling policy for a multi-cluster warehouse that determines when additional clusters are started or shut down.
  name: scaling_policy
  type: string
- description: Number of seconds of inactivity after which a warehouse is automatically suspended. A value of 0 means the warehouse is never automatically suspended.
  name: auto_suspend
  type: integer
- description: Specifies whether to automatically resume a warehouse when a SQL statement is submitted to it.
  name: auto_resume
  type: string
- description: Specifies whether the warehouse is created initially in the Suspended state.
  name: initially_suspended
  type: string
- description: Specifies the name of a resource monitor that is explicitly assigned to the warehouse. When a resource monitor is explicitly assigned, the monitor controls the monthly credits used by the warehouse.
  name: resource_monitor
  type: string
- description: Specifies a comment for the warehouse.
  name: comment
  type: string
- description: Specifies whether to enable the query acceleration service for queries that rely on this warehouse for compute resources.
  name: enable_query_acceleration
  type: string
- description: Specifies the maximum scale factor for leasing compute resources for query acceleration. The scale factor is used as a multiplier based on warehouse size.
  name: query_acceleration_max_scale_factor
  type: integer
- description: Object parameter that specifies the concurrency level for SQL statements executed by a warehouse cluster.
  name: max_concurrency_level
  type: integer
- description: Object parameter that specifies the time, in seconds, a SQL statement can be queued on a warehouse before it is canceled by the system.
  name: statement_queued_timeout_in_seconds
  type: integer
- description: Object parameter that specifies the time, in seconds, after which a running SQL statement is canceled by the system.
  name: statement_timeout_in_seconds
  type: integer
- description: Credit limit that can be consumed by the warehouse.
  name: warehouse_credit_limit
  type: integer
- description: Target statement size for adaptive warehouses.
  name: target_statement_size
  type: string
- description: The current state of the warehouse.
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
- description: Whether the warehouse is in use for the session. Only one warehouse can be in use at a time for a session.
  name: is_current
  type: boolean
- description: Percentage of the warehouse compute resources that are provisioned and available.
  name: available
  type: string
- description: Percentage of the warehouse compute resources that are in the process of provisioning.
  name: provisioning
  type: string
- description: Percentage of the warehouse compute resources that are executing SQL statements but will be shut down once the queries complete.
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
- description: Date and time when the warehouse was last updated, which includes changing any of the properties of the warehouse or changing the state.
  name: updated_on
  type: string
- description: Role that owns the warehouse.
  name: owner
  type: string
- description: The type of role that owns the object.
  name: owner_role_type
  type: string
- description: Budget associated with the warehouse.
  name: budget
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/snowflake-warehouse-schema.json
slug: snowflake-warehouse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-warehouse-schema.json\",\n  \"title\": \"Snowflake Warehouse\",\n  \"description\": \"A Snowflake virtual warehouse provides the compute resources required to execute queries and perform DML operations. A warehouse can be started, suspended, resized, and configured for auto-suspend and auto-resume.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the virtual warehouse. Must be unique within the account.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"warehouse_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of warehouse specifying the compute resource architecture.\",\n      \"enum\": [\n        \"STANDARD\",\n        \"SNOWPARK-OPTIMIZED\"\n      ],\n      \"default\":\
  \ \"STANDARD\"\n    },\n    \"warehouse_size\": {\n      \"type\": \"string\",\n      \"description\": \"Size of the warehouse determining the number of compute resources per cluster.\",\n      \"enum\": [\n        \"XSMALL\",\n        \"SMALL\",\n        \"MEDIUM\",\n        \"LARGE\",\n        \"XLARGE\",\n        \"XXLARGE\",\n        \"XXXLARGE\",\n        \"X4LARGE\",\n        \"X5LARGE\",\n        \"X6LARGE\"\n      ]\n    },\n    \"wait_for_completion\": {\n      \"type\": \"string\",\n      \"description\": \"When resizing a warehouse, block the return of the ALTER WAREHOUSE command until the resize has finished provisioning all its compute resources.\",\n      \"enum\": [\n        \"true\",\n        \"false\"\n      ]\n    },\n    \"max_cluster_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Specifies the maximum number of clusters for a multi-cluster warehouse. For a single-cluster warehouse, this value is 1.\",\n      \"minimum\": 1,\n      \"maximum\": 10\n\
  \    },\n    \"min_cluster_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Specifies the minimum number of clusters for a multi-cluster warehouse. For a single-cluster warehouse, this value is 1.\",\n      \"minimum\": 1,\n      \"maximum\": 10\n    },\n    \"scaling_policy\": {\n      \"type\": \"string\",\n      \"description\": \"Scaling policy for a multi-cluster warehouse that determines when additional clusters are started or shut down.\",\n      \"enum\": [\n        \"STANDARD\",\n        \"ECONOMY\"\n      ],\n      \"default\": \"STANDARD\"\n    },\n    \"auto_suspend\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of seconds of inactivity after which a warehouse is automatically suspended. A value of 0 means the warehouse is never automatically suspended.\",\n      \"minimum\": 0\n    },\n    \"auto_resume\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies whether to automatically resume a warehouse when a SQL statement\
  \ is submitted to it.\",\n      \"enum\": [\n        \"true\",\n        \"false\"\n      ]\n    },\n    \"initially_suspended\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies whether the warehouse is created initially in the Suspended state.\",\n      \"enum\": [\n        \"true\",\n        \"false\"\n      ]\n    },\n    \"resource_monitor\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the name of a resource monitor that is explicitly assigned to the warehouse. When a resource monitor is explicitly assigned, the monitor controls the monthly credits used by the warehouse.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies a comment for the warehouse.\"\n    },\n    \"enable_query_acceleration\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies whether to enable the query acceleration service for queries that rely on this warehouse for compute resources.\",\n      \"enum\": [\n    \
  \    \"true\",\n        \"false\"\n      ]\n    },\n    \"query_acceleration_max_scale_factor\": {\n      \"type\": \"integer\",\n      \"description\": \"Specifies the maximum scale factor for leasing compute resources for query acceleration. The scale factor is used as a multiplier based on warehouse size.\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"max_concurrency_level\": {\n      \"type\": \"integer\",\n      \"description\": \"Object parameter that specifies the concurrency level for SQL statements executed by a warehouse cluster.\",\n      \"minimum\": 1\n    },\n    \"statement_queued_timeout_in_seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Object parameter that specifies the time, in seconds, a SQL statement can be queued on a warehouse before it is canceled by the system.\",\n      \"minimum\": 0\n    },\n    \"statement_timeout_in_seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Object parameter that specifies the\
  \ time, in seconds, after which a running SQL statement is canceled by the system.\",\n      \"minimum\": 0\n    },\n    \"warehouse_credit_limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Credit limit that can be consumed by the warehouse.\"\n    },\n    \"target_statement_size\": {\n      \"type\": \"string\",\n      \"description\": \"Target statement size for adaptive warehouses.\",\n      \"enum\": [\n        \"X-Small\",\n        \"Small\",\n        \"Medium\",\n        \"Large\",\n        \"X-Large\",\n        \"2X-Large\",\n        \"3X-Large\",\n        \"4X-Large\",\n        \"5X-Large\",\n        \"6X-Large\"\n      ]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the warehouse.\",\n      \"enum\": [\n        \"STARTED\",\n        \"STARTING\",\n        \"DYNAMIC\",\n        \"SUSPENDED\",\n        \"RESIZING\",\n        \"RESUMING\",\n        \"SUSPENDING\"\n      ],\n      \"readOnly\": true\n    },\n\
  \    \"started_clusters\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of clusters currently started.\",\n      \"readOnly\": true\n    },\n    \"running\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of SQL statements that are being executed by the warehouse.\",\n      \"readOnly\": true\n    },\n    \"queued\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of SQL statements that are queued for the warehouse.\",\n      \"readOnly\": true\n    },\n    \"is_default\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the warehouse is the default for the current user.\",\n      \"readOnly\": true\n    },\n    \"is_current\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the warehouse is in use for the session. Only one warehouse can be in use at a time for a session.\",\n      \"readOnly\": true\n    },\n    \"available\": {\n      \"type\": \"string\",\n      \"description\": \"Percentage of\
  \ the warehouse compute resources that are provisioned and available.\",\n      \"readOnly\": true\n    },\n    \"provisioning\": {\n      \"type\": \"string\",\n      \"description\": \"Percentage of the warehouse compute resources that are in the process of provisioning.\",\n      \"readOnly\": true\n    },\n    \"quiescing\": {\n      \"type\": \"string\",\n      \"description\": \"Percentage of the warehouse compute resources that are executing SQL statements but will be shut down once the queries complete.\",\n      \"readOnly\": true\n    },\n    \"other\": {\n      \"type\": \"string\",\n      \"description\": \"Percentage of the warehouse compute resources that are in a state other than available, provisioning, or quiescing.\",\n      \"readOnly\": true\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the warehouse was created.\",\n      \"readOnly\": true\n    },\n    \"resumed_on\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the warehouse was last started or restarted.\",\n      \"readOnly\": true\n    },\n    \"updated_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the warehouse was last updated, which includes changing any of the properties of the warehouse or changing the state.\",\n      \"readOnly\": true\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Role that owns the warehouse.\",\n      \"readOnly\": true\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the object.\",\n      \"readOnly\": true\n    },\n    \"budget\": {\n      \"type\": \"string\",\n      \"description\": \"Budget associated with the warehouse.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"additionalProperties\": false\n\
  }\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-warehouse-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Snowflake Warehouse
---
