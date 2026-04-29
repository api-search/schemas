---
description: ''
layout: schema
name: SubStatementData
properties_list:
- description: The identifier of the sub-statement
  name: Id
  type: string
- description: The status of the sub-statement
  name: Status
  type: string
- description: The date and time the sub-statement was created
  name: CreatedAt
  type: string
- description: The date and time the sub-statement was last updated
  name: UpdatedAt
  type: string
- description: The time in nanoseconds the sub-statement ran
  name: Duration
  type: integer
- description: The SQL statement text
  name: QueryString
  type: string
- description: The Redshift query identifier
  name: RedshiftQueryId
  type: integer
- description: Total number of rows in the result set
  name: ResultRows
  type: integer
- description: The size of the result set in bytes
  name: ResultSize
  type: integer
- description: Whether the sub-statement has a result set
  name: HasResultSet
  type: boolean
- description: The error message if the sub-statement failed
  name: Error
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-sub-statement-data-schema.json
slug: amazon-redshift-data-sub-statement-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubStatementData\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the sub-statement\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the sub-statement\"\n    },\n    \"CreatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the sub-statement was created\"\n    },\n    \"UpdatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the sub-statement was last updated\"\n    },\n    \"Duration\": {\n      \"type\": \"integer\",\n      \"description\": \"The time in nanoseconds the sub-statement ran\"\n    },\n    \"QueryString\": {\n      \"type\": \"string\",\n      \"description\": \"The SQL statement text\"\n    },\n    \"RedshiftQueryId\": {\n      \"type\": \"integer\",\n      \"description\": \"The\
  \ Redshift query identifier\"\n    },\n    \"ResultRows\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of rows in the result set\"\n    },\n    \"ResultSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the result set in bytes\"\n    },\n    \"HasResultSet\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the sub-statement has a result set\"\n    },\n    \"Error\": {\n      \"type\": \"string\",\n      \"description\": \"The error message if the sub-statement failed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-sub-statement-data-schema.json
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
title: SubStatementData
---
