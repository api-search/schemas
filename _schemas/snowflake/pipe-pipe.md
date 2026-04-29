---
description: A Snowflake pipe
layout: schema
name: Pipe
properties_list:
- description: Name of the pipe
  name: name
  type: string
- description: user comment associated to an object in the dictionary
  name: comment
  type: string
- description: TRUE if all files from stage need to be auto-ingested
  name: auto_ingest
  type: boolean
- description: Link to integration object that point to a user provided Azure storage queue / SQS. When present, errors (e.g. ingest failure for Snowpipe or a user task failure or replication failure) will be sent t
  name: error_integration
  type: string
- description: Optional, if provided, auto_ingest pipe will only receive messages from this SNS topic.
  name: aws_sns_topic
  type: string
- description: Link to integration object that ties a user provided storage queue to an auto_ingest enabled pipe. Required for auto_ingest to work on azure.
  name: integration
  type: string
- description: COPY INTO <table> statement used to load data from queued files into a Snowflake table. This statement serves as the text/definition for the pipe and is displayed in the SHOW PIPES output
  name: copy_statement
  type: string
- description: Date and time when the pipe was created.
  name: created_on
  type: string
- description: Database in which the pipe is stored
  name: database_name
  type: string
- description: Schema in which the pipe is stored
  name: schema_name
  type: string
- description: Role that owns the pipe
  name: owner
  type: string
- description: PATTERN copy option value in the COPY INTO <table> statement in the pipe definition, if the copy option was specified.
  name: pattern
  type: string
- description: The type of role that owns the pipe
  name: owner_role_type
  type: string
- description: Displays some detailed information for your pipes that may have issues
  name: invalid_reason
  type: string
- description: Name of the budget if the pipe is monitored by a budget
  name: budget
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/pipe-pipe-schema.json
slug: pipe-pipe
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Pipe\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake pipe\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the pipe\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"user comment associated to an object in the dictionary\"\n    },\n    \"auto_ingest\": {\n      \"type\": \"boolean\",\n      \"description\": \"TRUE if all files from stage need to be auto-ingested\"\n    },\n    \"error_integration\": {\n      \"type\": \"string\",\n      \"description\": \"Link to integration object that point to a user provided Azure storage queue / SQS. When present,  errors (e.g. ingest failure for Snowpipe or a user task failure or replication failure) will be sent to this queue to notify customers\"\n    },\n    \"aws_sns_topic\": {\n      \"type\": \"string\",\n      \"description\": \"Optional, if provided,\
  \ auto_ingest pipe will only receive messages from this SNS topic.\"\n    },\n    \"integration\": {\n      \"type\": \"string\",\n      \"description\": \"Link to integration object that ties a user provided storage queue to an auto_ingest enabled pipe. Required for auto_ingest to work on azure.\"\n    },\n    \"copy_statement\": {\n      \"type\": \"string\",\n      \"description\": \"COPY INTO <table> statement used to load data from queued files into a Snowflake table. This statement serves as the text/definition for the pipe and is displayed in the SHOW PIPES output\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the pipe was created.\"\n    },\n    \"database_name\": {\n      \"type\": \"string\",\n      \"description\": \"Database in which the pipe is stored\"\n    },\n    \"schema_name\": {\n      \"type\": \"string\",\n      \"description\": \"Schema in which the pipe is stored\"\n    },\n    \"owner\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Role that owns the pipe\"\n    },\n    \"pattern\": {\n      \"type\": \"string\",\n      \"description\": \"PATTERN copy option value in the COPY INTO <table> statement in the pipe definition, if the copy option was specified.\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the pipe\"\n    },\n    \"invalid_reason\": {\n      \"type\": \"string\",\n      \"description\": \"Displays some detailed information for your pipes that may have issues\"\n    },\n    \"budget\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the budget if the pipe is monitored by a budget\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/pipe-pipe-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Pipe
---
