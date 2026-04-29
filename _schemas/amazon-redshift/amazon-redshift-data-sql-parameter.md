---
description: ''
layout: schema
name: SqlParameter
properties_list:
- description: The name of the parameter (without the colon prefix)
  name: name
  type: string
- description: The value of the parameter
  name: value
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-sql-parameter-schema.json
slug: amazon-redshift-data-sql-parameter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SqlParameter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the parameter (without the colon prefix)\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the parameter\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-sql-parameter-schema.json
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
title: SqlParameter
---
