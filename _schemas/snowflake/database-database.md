---
description: Snowflake database object.
layout: schema
name: Database
properties_list:
- description: Date and time the database was created.
  name: created_on
  type: string
- description: Database type, permanent (default) or transient.
  name: kind
  type: string
- description: Whether the database is the default database for a user.
  name: is_default
  type: boolean
- description: Current database for the session.
  name: is_current
  type: boolean
- description: ''
  name: origin
  type: string
- description: Name of the role that owns the database.
  name: owner
  type: string
- description: Optional comment in which to store information related to the database.
  name: comment
  type: string
- description: ''
  name: options
  type: string
- description: Number of days that historical data is retained for Time Travel.
  name: retention_time
  type: integer
- description: Date and time the database was dropped.
  name: dropped_on
  type: string
- description: Budget that defines a monthly spending limit on the compute costs for a Snowflake account or a custom group of Snowflake objects.
  name: budget
  type: string
- description: Type of role that owns the object, either ROLE or DATABASE_ROLE
  name: owner_role_type
  type: string
- description: 'Specifies the number of days for which Time Travel actions (CLONE and UNDROP) can be performed on the database, as well as specifying the default Time Travel retention time for all schemas created in '
  name: data_retention_time_in_days
  type: integer
- description: Default collation specification for all schemas and tables added to the database. You an override the default at the schema and individual table levels.
  name: default_ddl_collation
  type: string
- description: Severity level of messages that should be ingested and made available in the active event table. Currently, Snowflake supports only `TRACE`, `DEBUG`, `INFO`, `WARN`, `ERROR`, `FATAL` and `OFF`.
  name: log_level
  type: string
- description: Maximum number of days for which Snowflake can extend the data retention period for tables in the database to prevent streams on the tables from becoming stale.
  name: max_data_extension_time_in_days
  type: integer
- description: Maximum number of consecutive failed task runs before the current task is suspended automatically.
  name: suspend_task_after_num_failures
  type: integer
- description: How trace events are ingested into the event table. Currently, Snowflake supports only `ALWAYS`, `ON_EVENT`, and `OFF`.
  name: trace_level
  type: string
- description: Size of the compute resources to provision for the first run of the serverless task, before a task history is available for Snowflake to determine an ideal size.
  name: user_task_managed_initial_warehouse_size
  type: string
- description: Time limit, in milliseconds, for a single run of the task before it times out.
  name: user_task_timeout_ms
  type: integer
- description: Specifies the minimum allowed warehouse size for the serverless task. Minimum XSMALL, Maximum XXLARGE.
  name: serverless_task_min_statement_size
  type: string
- description: Specifies the maximum allowed warehouse size for the serverless task. Minimum XSMALL, Maximum XXLARGE.
  name: serverless_task_max_statement_size
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/database-database-schema.json
slug: database-database
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Database\",\n  \"type\": \"object\",\n  \"description\": \"Snowflake database object.\",\n  \"properties\": {\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time the database was created.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Database type, permanent (default) or transient.\"\n    },\n    \"is_default\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the database is the default database for a user.\"\n    },\n    \"is_current\": {\n      \"type\": \"boolean\",\n      \"description\": \"Current database for the session.\"\n    },\n    \"origin\": {\n      \"type\": \"string\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the role that owns the database.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional comment\
  \ in which to store information related to the database.\"\n    },\n    \"options\": {\n      \"type\": \"string\"\n    },\n    \"retention_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of days that historical data is retained for Time Travel.\"\n    },\n    \"dropped_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time the database was dropped.\"\n    },\n    \"budget\": {\n      \"type\": \"string\",\n      \"description\": \"Budget that defines a monthly spending limit on the compute costs for a Snowflake account or a custom group of Snowflake objects.\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of role that owns the object, either ROLE or DATABASE_ROLE\"\n    },\n    \"data_retention_time_in_days\": {\n      \"type\": \"integer\",\n      \"description\": \"Specifies the number of days for which Time Travel actions (CLONE and UNDROP) can be performed on the database, as well as specifying\
  \ the default Time Travel retention time for all schemas created in the database.\"\n    },\n    \"default_ddl_collation\": {\n      \"type\": \"string\",\n      \"description\": \"Default collation specification for all schemas and tables added to the database. You an override the default at the schema and individual table levels.\"\n    },\n    \"log_level\": {\n      \"type\": \"string\",\n      \"description\": \"Severity level of messages that should be ingested and made available in the active event table. Currently, Snowflake supports only `TRACE`, `DEBUG`, `INFO`, `WARN`, `ERROR`, `FATAL` and `OFF`.\"\n    },\n    \"max_data_extension_time_in_days\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of days for which Snowflake can extend the data retention period for tables in the database to prevent streams on the tables from becoming stale.\"\n    },\n    \"suspend_task_after_num_failures\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum\
  \ number of consecutive failed task runs before the current task is suspended automatically.\"\n    },\n    \"trace_level\": {\n      \"type\": \"string\",\n      \"description\": \"How trace events are ingested into the event table. Currently, Snowflake supports only `ALWAYS`, `ON_EVENT`, and `OFF`.\"\n    },\n    \"user_task_managed_initial_warehouse_size\": {\n      \"type\": \"string\",\n      \"description\": \"Size of the compute resources to provision for the first run of the serverless task, before a task history is available for Snowflake to determine an ideal size.\"\n    },\n    \"user_task_timeout_ms\": {\n      \"type\": \"integer\",\n      \"description\": \"Time limit, in milliseconds, for a single run of the task before it times out.\"\n    },\n    \"serverless_task_min_statement_size\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the minimum allowed warehouse size for the serverless task. Minimum XSMALL, Maximum XXLARGE.\"\n    },\n    \"serverless_task_max_statement_size\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Specifies the maximum allowed warehouse size for the serverless task. Minimum XSMALL, Maximum XXLARGE.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/database-database-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Database
---
