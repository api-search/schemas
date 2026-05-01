---
description: A Timestream database resource containing tables for time series data storage.
layout: schema
name: Database
properties_list:
- description: The Amazon Resource Name that uniquely identifies this database.
  name: Arn
  type: string
- description: The name of the Timestream database.
  name: DatabaseName
  type: string
- description: The total number of tables found within the Timestream database.
  name: TableCount
  type: integer
- description: The identifier of the KMS key used to encrypt the data stored in the database.
  name: KmsKeyId
  type: string
- description: The time when the database was created.
  name: CreationTime
  type: string
- description: The last time that this database was updated.
  name: LastUpdatedTime
  type: string
provider_name: Amazon Timestream
provider_slug: amazon-timestream
schema_file: json-schema/amazon-timestream-database-schema.json
slug: amazon-timestream-database
source_filename: amazon-timestream-database-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A Timestream database resource containing tables for time series data storage.\",\n  \"properties\": {\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name that uniquely identifies this database.\"\n    },\n    \"DatabaseName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Timestream database.\"\n    },\n    \"TableCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of tables found within the Timestream database.\"\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the KMS key used to encrypt the data stored in the database.\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the database was created.\"\n    },\n    \"LastUpdatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"The last time that this database was updated.\"\n    }\n  },\n  \"required\": [\n    \"Arn\",\n    \"DatabaseName\"\n  ],\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Database\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-timestream/refs/heads/main/json-schema/amazon-timestream-database-schema.json
tags:
- Database
- Iot
- Time Series
title: Database
---
