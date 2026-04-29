---
description: A database in the AWS Glue Data Catalog managed by Lake Formation.
layout: schema
name: Database
properties_list:
- description: The name of the database.
  name: Name
  type: string
- description: The ID of the Data Catalog.
  name: CatalogId
  type: string
- description: A description of the database.
  name: Description
  type: string
- description: The location of the database (for example, an HDFS path).
  name: LocationUri
  type: string
- description: The time at which the metadata database was created.
  name: CreateTime
  type: string
provider_name: AWS Lake Formation
provider_slug: amazon-lakeformation
schema_file: json-schema/amazon-lakeformation-database-schema.json
slug: amazon-lakeformation-database
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lakeformation/refs/heads/main/json-schema/amazon-lakeformation-database-schema.json\",\n  \"title\": \"Database\",\n  \"description\": \"A database in the AWS Glue Data Catalog managed by Lake Formation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database.\",\n      \"example\": \"my_analytics_db\"\n    },\n    \"CatalogId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Data Catalog.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the database.\"\n    },\n    \"LocationUri\": {\n      \"type\": \"string\",\n      \"description\": \"The location of the database (for example, an HDFS path).\"\n    },\n    \"CreateTime\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The time at which the metadata database was created.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lakeformation/refs/heads/main/json-schema/amazon-lakeformation-database-schema.json
tags:
- Analytics
- AWS
- Data Lake
- Governance
title: Database
---
