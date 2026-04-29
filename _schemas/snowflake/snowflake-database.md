---
description: A Snowflake database is a logical grouping of schemas, which in turn contain database objects such as tables, views, and stages. Databases support features like cloning, replication, failover, Time Travel, and data sharing.
layout: schema
name: Snowflake Database
properties_list:
- description: Identifier for the database. Must be unique within the account.
  name: name
  type: string
- description: Database type. Permanent databases persist until explicitly dropped. Transient databases exist for the duration of the user session and do not have a Fail-safe period.
  name: kind
  type: string
- description: Optional comment in which to store information related to the database.
  name: comment
  type: string
- description: 'Specifies the number of days for which Time Travel actions (CLONE and UNDROP) can be performed on the database, as well as specifying the default Time Travel retention time for all schemas created in '
  name: data_retention_time_in_days
  type: integer
- description: Default collation specification for all schemas and tables added to the database. You can override the default at the schema and individual table levels.
  name: default_ddl_collation
  type: string
- description: Severity level of messages that should be ingested and made available in the active event table.
  name: log_level
  type: string
- description: Maximum number of days for which Snowflake can extend the data retention period for tables in the database to prevent streams on the tables from becoming stale.
  name: max_data_extension_time_in_days
  type: integer
- description: Maximum number of consecutive failed task runs before the current task is suspended automatically.
  name: suspend_task_after_num_failures
  type: integer
- description: How trace events are ingested into the event table.
  name: trace_level
  type: string
- description: Size of the compute resources to provision for the first run of the serverless task, before a task history is available for Snowflake to determine an ideal size.
  name: user_task_managed_initial_warehouse_size
  type: string
- description: Time limit, in milliseconds, for a single run of the task before it times out.
  name: user_task_timeout_ms
  type: integer
- description: Specifies the minimum allowed warehouse size for the serverless task.
  name: serverless_task_min_statement_size
  type: string
- description: Specifies the maximum allowed warehouse size for the serverless task.
  name: serverless_task_max_statement_size
  type: string
- description: Date and time the database was created.
  name: created_on
  type: string
- description: Whether the database is the default database for a user.
  name: is_default
  type: boolean
- description: Whether the database is the current database for the session.
  name: is_current
  type: boolean
- description: For a database created from a share, the fully qualified name of the source database.
  name: origin
  type: string
- description: Name of the role that owns the database.
  name: owner
  type: string
- description: Type of role that owns the object, either ROLE or DATABASE_ROLE.
  name: owner_role_type
  type: string
- description: Options set on the database.
  name: options
  type: string
- description: Number of days that historical data is retained for Time Travel.
  name: retention_time
  type: integer
- description: Date and time the database was dropped. Null if the database has not been dropped.
  name: dropped_on
  type:
  - string
  - 'null'
- description: Budget that defines a monthly spending limit on the compute costs for a Snowflake account or a custom group of Snowflake objects.
  name: budget
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/snowflake-database-schema.json
slug: snowflake-database
source_filename: snowflake-database-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-database-schema.json\",\n  \"title\": \"Snowflake Database\",\n  \"description\": \"A Snowflake database is a logical grouping of schemas, which in turn contain database objects such as tables, views, and stages. Databases support features like cloning, replication, failover, Time Travel, and data sharing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the database. Must be unique within the account.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Database type. Permanent databases persist until explicitly dropped. Transient databases exist for the duration of the user session and do not have a Fail-safe period.\",\n      \"enum\"\
  : [\n        \"PERMANENT\",\n        \"TRANSIENT\"\n      ],\n      \"default\": \"PERMANENT\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional comment in which to store information related to the database.\"\n    },\n    \"data_retention_time_in_days\": {\n      \"type\": \"integer\",\n      \"description\": \"Specifies the number of days for which Time Travel actions (CLONE and UNDROP) can be performed on the database, as well as specifying the default Time Travel retention time for all schemas created in the database.\",\n      \"minimum\": 0,\n      \"maximum\": 90\n    },\n    \"default_ddl_collation\": {\n      \"type\": \"string\",\n      \"description\": \"Default collation specification for all schemas and tables added to the database. You can override the default at the schema and individual table levels.\"\n    },\n    \"log_level\": {\n      \"type\": \"string\",\n      \"description\": \"Severity level of messages that should be ingested\
  \ and made available in the active event table.\",\n      \"enum\": [\n        \"TRACE\",\n        \"DEBUG\",\n        \"INFO\",\n        \"WARN\",\n        \"ERROR\",\n        \"FATAL\",\n        \"OFF\"\n      ]\n    },\n    \"max_data_extension_time_in_days\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of days for which Snowflake can extend the data retention period for tables in the database to prevent streams on the tables from becoming stale.\",\n      \"minimum\": 0,\n      \"maximum\": 90\n    },\n    \"suspend_task_after_num_failures\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of consecutive failed task runs before the current task is suspended automatically.\",\n      \"minimum\": 0\n    },\n    \"trace_level\": {\n      \"type\": \"string\",\n      \"description\": \"How trace events are ingested into the event table.\",\n      \"enum\": [\n        \"ALWAYS\",\n        \"ON_EVENT\",\n        \"OFF\"\n      ]\n   \
  \ },\n    \"user_task_managed_initial_warehouse_size\": {\n      \"type\": \"string\",\n      \"description\": \"Size of the compute resources to provision for the first run of the serverless task, before a task history is available for Snowflake to determine an ideal size.\",\n      \"enum\": [\n        \"XSMALL\",\n        \"SMALL\",\n        \"MEDIUM\",\n        \"LARGE\",\n        \"XLARGE\",\n        \"XXLARGE\"\n      ]\n    },\n    \"user_task_timeout_ms\": {\n      \"type\": \"integer\",\n      \"description\": \"Time limit, in milliseconds, for a single run of the task before it times out.\",\n      \"minimum\": 0\n    },\n    \"serverless_task_min_statement_size\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the minimum allowed warehouse size for the serverless task.\",\n      \"enum\": [\n        \"XSMALL\",\n        \"SMALL\",\n        \"MEDIUM\",\n        \"LARGE\",\n        \"XLARGE\",\n        \"XXLARGE\"\n      ]\n    },\n    \"serverless_task_max_statement_size\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Specifies the maximum allowed warehouse size for the serverless task.\",\n      \"enum\": [\n        \"XSMALL\",\n        \"SMALL\",\n        \"MEDIUM\",\n        \"LARGE\",\n        \"XLARGE\",\n        \"XXLARGE\"\n      ]\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the database was created.\",\n      \"readOnly\": true\n    },\n    \"is_default\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the database is the default database for a user.\",\n      \"readOnly\": true\n    },\n    \"is_current\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the database is the current database for the session.\",\n      \"readOnly\": true\n    },\n    \"origin\": {\n      \"type\": \"string\",\n      \"description\": \"For a database created from a share, the fully qualified name of the source database.\",\n   \
  \   \"readOnly\": true\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the role that owns the database.\",\n      \"readOnly\": true\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of role that owns the object, either ROLE or DATABASE_ROLE.\",\n      \"readOnly\": true\n    },\n    \"options\": {\n      \"type\": \"string\",\n      \"description\": \"Options set on the database.\",\n      \"readOnly\": true\n    },\n    \"retention_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of days that historical data is retained for Time Travel.\",\n      \"readOnly\": true\n    },\n    \"dropped_on\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the database was dropped. Null if the database has not been dropped.\",\n      \"readOnly\": true\n    },\n    \"budget\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Budget that defines a monthly spending limit on the compute costs for a Snowflake account or a custom group of Snowflake objects.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-database-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Snowflake Database
---
