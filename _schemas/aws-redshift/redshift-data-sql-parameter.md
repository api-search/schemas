---
description: A parameter used in a SQL statement.
layout: schema
name: SqlParameter
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: value
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-data-sql-parameter-schema.json
slug: redshift-data-sql-parameter
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {},\n    \"value\": {}\n  },\n  \"required\": [\n    \"name\",\n    \"value\"\n  ],\n  \"description\": \"A parameter used in a SQL statement.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-sql-parameter-schema.json\",\n  \"title\": \"SqlParameter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-sql-parameter-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: SqlParameter
---
