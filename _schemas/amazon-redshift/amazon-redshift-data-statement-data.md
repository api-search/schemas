---
description: ''
layout: schema
name: StatementData
properties_list:
- description: The identifier of the SQL statement
  name: Id
  type: string
- description: The name of the SQL statement
  name: StatementName
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
- description: The SQL statement text
  name: QueryString
  type: string
- description: The query parameters
  name: QueryParameters
  type: array
- description: The name of the database
  name: Database
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
- description: Whether this is a batch statement
  name: IsBatchStatement
  type: boolean
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-statement-data-schema.json
slug: amazon-redshift-data-statement-data
source_filename: amazon-redshift-data-statement-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatementData\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the SQL statement\"\n    },\n    \"StatementName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the SQL statement\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the SQL statement\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the statement was created\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the statement was last updated\"\n    },\n    \"QueryString\": {\n      \"type\": \"string\",\n      \"description\": \"The SQL statement text\"\n    },\n    \"QueryParameters\": {\n      \"type\": \"array\",\n      \"description\": \"The query parameters\"\n  \
  \  },\n    \"Database\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database\"\n    },\n    \"ClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The cluster identifier\"\n    },\n    \"WorkgroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The serverless workgroup name\"\n    },\n    \"SecretArn\": {\n      \"type\": \"string\",\n      \"description\": \"The secret ARN\"\n    },\n    \"IsBatchStatement\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a batch statement\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-statement-data-schema.json
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
title: StatementData
---
