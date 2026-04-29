---
description: ''
layout: schema
name: DescribeStatementResponse
properties_list:
- description: The identifier of the SQL statement
  name: Id
  type: string
- description: The status of the SQL statement
  name: Status
  type: string
- description: The date and time the statement was created
  name: CreatedAt
  type: string
- description: The date and time the statement was last updated
  name: UpdatedAt
  type: string
- description: The time in nanoseconds the statement ran
  name: Duration
  type: integer
- description: The SQL statement that was executed
  name: QueryString
  type: string
- description: The parameters for the SQL statement
  name: QueryParameters
  type: array
- description: The name of the database
  name: Database
  type: string
- description: The database user
  name: DbUser
  type: string
- description: The cluster identifier
  name: ClusterIdentifier
  type: string
- description: The serverless workgroup name
  name: WorkgroupName
  type: string
- description: The secret ARN
  name: SecretArn
  type: string
- description: The process identifier from the Redshift cluster
  name: RedshiftPid
  type: integer
- description: The Redshift query identifier
  name: RedshiftQueryId
  type: integer
- description: Total number of rows in the result set (FINISHED only)
  name: ResultRows
  type: integer
- description: The size of the result set in bytes
  name: ResultSize
  type: integer
- description: Whether the statement has a result set
  name: HasResultSet
  type: boolean
- description: The error message if the statement failed
  name: Error
  type: string
- description: List of sub-statements for a batch execution. Only present for BatchExecuteStatement calls.
  name: SubStatements
  type: array
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-describe-statement-response-schema.json
slug: amazon-redshift-data-describe-statement-response
source_filename: amazon-redshift-data-describe-statement-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeStatementResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the SQL statement\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the SQL statement\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the statement was created\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the statement was last updated\"\n    },\n    \"Duration\": {\n      \"type\": \"integer\",\n      \"description\": \"The time in nanoseconds the statement ran\"\n    },\n    \"QueryString\": {\n      \"type\": \"string\",\n      \"description\": \"The SQL statement that was executed\"\n    },\n    \"QueryParameters\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"The parameters for the SQL statement\"\n    },\n    \"Database\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database\"\n    },\n    \"DbUser\": {\n      \"type\": \"string\",\n      \"description\": \"The database user\"\n    },\n    \"ClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The cluster identifier\"\n    },\n    \"WorkgroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The serverless workgroup name\"\n    },\n    \"SecretArn\": {\n      \"type\": \"string\",\n      \"description\": \"The secret ARN\"\n    },\n    \"RedshiftPid\": {\n      \"type\": \"integer\",\n      \"description\": \"The process identifier from the Redshift cluster\"\n    },\n    \"RedshiftQueryId\": {\n      \"type\": \"integer\",\n      \"description\": \"The Redshift query identifier\"\n    },\n    \"ResultRows\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of rows in the result set (FINISHED only)\"\
  \n    },\n    \"ResultSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the result set in bytes\"\n    },\n    \"HasResultSet\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the statement has a result set\"\n    },\n    \"Error\": {\n      \"type\": \"string\",\n      \"description\": \"The error message if the statement failed\"\n    },\n    \"SubStatements\": {\n      \"type\": \"array\",\n      \"description\": \"List of sub-statements for a batch execution. Only present for BatchExecuteStatement calls.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-describe-statement-response-schema.json
tags:
- Analytics
- Big Data
- Cloud
- Data Lake
- Data Warehouse
- ETL
- Machine Learning
- Serverless
- SQL
title: DescribeStatementResponse
---
