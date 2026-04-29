---
description: ''
layout: schema
name: ExecuteStatementRequest
properties_list:
- description: The cluster identifier. Required when connecting to a provisioned cluster. Mutually exclusive with WorkgroupName.
  name: ClusterIdentifier
  type: string
- description: The name of the database to run the SQL statement against
  name: Database
  type: string
- description: The database user name. Required when authenticating with temporary credentials from GetClusterCredentials.
  name: DbUser
  type: string
- description: The ARN of the secret stored in AWS Secrets Manager that contains the database credentials. Mutually exclusive with DbUser and temporary credentials.
  name: SecretArn
  type: string
- description: The SQL statement to run. Maximum length is 100,000 characters.
  name: Sql
  type: string
- description: A name for the SQL statement. This name can be used to identify the query in the ListStatements output.
  name: StatementName
  type: string
- description: Whether to send an event to Amazon EventBridge when the SQL statement completes. Default is false.
  name: WithEvent
  type: boolean
- description: The serverless workgroup name. Required when connecting to Redshift Serverless. Mutually exclusive with ClusterIdentifier.
  name: WorkgroupName
  type: string
- description: Named parameters for the SQL statement. Use :name syntax in the SQL string to reference parameters.
  name: Parameters
  type: array
- description: A unique, case-sensitive identifier to ensure idempotency of the request.
  name: ClientToken
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-execute-statement-request-schema.json
slug: amazon-redshift-data-execute-statement-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExecuteStatementRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The cluster identifier. Required when connecting to a provisioned cluster. Mutually exclusive with WorkgroupName.\"\n    },\n    \"Database\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database to run the SQL statement against\"\n    },\n    \"DbUser\": {\n      \"type\": \"string\",\n      \"description\": \"The database user name. Required when authenticating with temporary credentials from GetClusterCredentials.\"\n    },\n    \"SecretArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the secret stored in AWS Secrets Manager that contains the database credentials. Mutually exclusive with DbUser and temporary credentials.\"\n    },\n    \"Sql\": {\n      \"type\": \"string\",\n  \
  \    \"description\": \"The SQL statement to run. Maximum length is 100,000 characters.\"\n    },\n    \"StatementName\": {\n      \"type\": \"string\",\n      \"description\": \"A name for the SQL statement. This name can be used to identify the query in the ListStatements output.\"\n    },\n    \"WithEvent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to send an event to Amazon EventBridge when the SQL statement completes. Default is false.\"\n    },\n    \"WorkgroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The serverless workgroup name. Required when connecting to Redshift Serverless. Mutually exclusive with ClusterIdentifier.\"\n    },\n    \"Parameters\": {\n      \"type\": \"array\",\n      \"description\": \"Named parameters for the SQL statement. Use :name syntax in the SQL string to reference parameters.\"\n    },\n    \"ClientToken\": {\n      \"type\": \"string\",\n      \"description\": \"A unique, case-sensitive identifier to ensure\
  \ idempotency of the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-execute-statement-request-schema.json
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
title: ExecuteStatementRequest
---
