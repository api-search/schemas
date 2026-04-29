---
description: ''
layout: schema
name: TableMember
properties_list:
- description: The name of the table
  name: name
  type: string
- description: The type of the table (TABLE, VIEW, etc.)
  name: type
  type: string
- description: The schema that contains the table
  name: schema
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-table-member-schema.json
slug: amazon-redshift-data-table-member
source_filename: amazon-redshift-data-table-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableMember\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the table (TABLE, VIEW, etc.)\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"The schema that contains the table\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-table-member-schema.json
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
title: TableMember
---
