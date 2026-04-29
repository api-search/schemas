---
description: Request body for submitting a SQL statement for execution.
layout: schema
name: StatementRequest
properties_list:
- description: 'SQL statement or batch of SQL statements to execute. You can specify query, DML and DDL statements. The following statements are not supported: PUT, GET, USE, ALTER SESSION, BEGIN, COMMIT, ROLLBACK, s'
  name: statement
  type: string
- description: Timeout in seconds for statement execution. If the execution of a statement takes longer than the specified timeout, the execution is automatically canceled. To set the timeout to the maximum value (6
  name: timeout
  type: integer
- description: Database in which the statement should be executed. The value in this field is case-sensitive.
  name: database
  type: string
- description: Schema in which the statement should be executed. The value in this field is case-sensitive.
  name: schema
  type: string
- description: Warehouse to use when executing the statement. The value in this field is case-sensitive.
  name: warehouse
  type: string
- description: Role to use when executing the statement. The value in this field is case-sensitive.
  name: role
  type: string
- description: Values of bind variables in the SQL statement. When executing the statement, Snowflake replaces placeholders (? and :name) in the statement with these specified values.
  name: bindings
  type: object
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/snowflake-sql-rest-statement-request-schema.json
slug: snowflake-sql-rest-statement-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatementRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for submitting a SQL statement for execution.\",\n  \"properties\": {\n    \"statement\": {\n      \"type\": \"string\",\n      \"description\": \"SQL statement or batch of SQL statements to execute. You can specify query, DML and DDL statements. The following statements are not supported: PUT, GET, USE, ALTER SESSION, BEGIN, COMMIT, ROLLBACK, statements that set session variables, and statements that create temporary tables and stages.\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in seconds for statement execution. If the execution of a statement takes longer than the specified timeout, the execution is automatically canceled. To set the timeout to the maximum value (604800 seconds), set timeout to 0.\"\n    },\n    \"database\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"Database in which the statement should be executed. The value in this field is case-sensitive.\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"Schema in which the statement should be executed. The value in this field is case-sensitive.\"\n    },\n    \"warehouse\": {\n      \"type\": \"string\",\n      \"description\": \"Warehouse to use when executing the statement. The value in this field is case-sensitive.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Role to use when executing the statement. The value in this field is case-sensitive.\"\n    },\n    \"bindings\": {\n      \"type\": \"object\",\n      \"description\": \"Values of bind variables in the SQL statement. When executing the statement, Snowflake replaces placeholders (? and :name) in the statement with these specified values.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-sql-rest-statement-request-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: StatementRequest
---
