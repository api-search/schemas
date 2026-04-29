---
description: SqlParametersList schema from Amazon Redshift
layout: schema
name: SqlParametersList
properties_list: []
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-data-sql-parameters-list-schema.json
slug: redshift-data-sql-parameters-list
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"name\": {},\n      \"value\": {}\n    },\n    \"required\": [\n      \"name\",\n      \"value\"\n    ],\n    \"description\": \"A parameter used in a SQL statement.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-sql-parameters-list-schema.json\",\n  \"title\": \"SqlParametersList\",\n  \"description\": \"SqlParametersList schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-sql-parameters-list-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: SqlParametersList
---
