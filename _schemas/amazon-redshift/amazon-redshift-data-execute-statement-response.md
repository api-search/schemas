---
description: ''
layout: schema
name: ExecuteStatementResponse
properties_list:
- description: The identifier of the SQL statement
  name: Id
  type: string
- description: The date and time the statement was created
  name: CreatedAt
  type: string
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
- description: The secret ARN used for authentication
  name: SecretArn
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-execute-statement-response-schema.json
slug: amazon-redshift-data-execute-statement-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExecuteStatementResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the SQL statement\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the statement was created\"\n    },\n    \"Database\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database\"\n    },\n    \"DbUser\": {\n      \"type\": \"string\",\n      \"description\": \"The database user\"\n    },\n    \"ClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The cluster identifier\"\n    },\n    \"WorkgroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The serverless workgroup name\"\n    },\n    \"SecretArn\": {\n      \"type\": \"string\",\n      \"description\": \"The secret ARN used for authentication\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-execute-statement-response-schema.json
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
title: ExecuteStatementResponse
---
