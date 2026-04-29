---
description: ''
layout: schema
name: BatchExecuteStatementRequest
properties_list:
- description: The cluster identifier for a provisioned cluster
  name: ClusterIdentifier
  type: string
- description: The name of the database
  name: Database
  type: string
- description: The database user name for temporary credentials
  name: DbUser
  type: string
- description: ARN of the secret in AWS Secrets Manager
  name: SecretArn
  type: string
- description: One or more SQL statements to run. The statements run serially as a single transaction. Maximum 40 statements.
  name: Sqls
  type: array
- description: A name for the batch SQL statement
  name: StatementName
  type: string
- description: Whether to send an event to EventBridge on completion
  name: WithEvent
  type: boolean
- description: The serverless workgroup name
  name: WorkgroupName
  type: string
- description: Idempotency token
  name: ClientToken
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-batch-execute-statement-request-schema.json
slug: amazon-redshift-data-batch-execute-statement-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchExecuteStatementRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The cluster identifier for a provisioned cluster\"\n    },\n    \"Database\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database\"\n    },\n    \"DbUser\": {\n      \"type\": \"string\",\n      \"description\": \"The database user name for temporary credentials\"\n    },\n    \"SecretArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the secret in AWS Secrets Manager\"\n    },\n    \"Sqls\": {\n      \"type\": \"array\",\n      \"description\": \"One or more SQL statements to run. The statements run serially as a single transaction. Maximum 40 statements.\"\n    },\n    \"StatementName\": {\n      \"type\": \"string\",\n      \"description\": \"A name for the batch SQL statement\"\n\
  \    },\n    \"WithEvent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to send an event to EventBridge on completion\"\n    },\n    \"WorkgroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The serverless workgroup name\"\n    },\n    \"ClientToken\": {\n      \"type\": \"string\",\n      \"description\": \"Idempotency token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-batch-execute-statement-request-schema.json
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
title: BatchExecuteStatementRequest
---
