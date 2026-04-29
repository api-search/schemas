---
description: The SQL statement to run.
layout: schema
name: StatementData
properties_list:
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: IsBatchStatement
  type: object
- description: ''
  name: QueryParameters
  type: object
- description: ''
  name: QueryString
  type: object
- description: ''
  name: QueryStrings
  type: object
- description: ''
  name: SecretArn
  type: object
- description: ''
  name: StatementName
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: UpdatedAt
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-data-statement-data-schema.json
slug: redshift-data-statement-data
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatedAt\": {},\n    \"Id\": {},\n    \"IsBatchStatement\": {},\n    \"QueryParameters\": {},\n    \"QueryString\": {},\n    \"QueryStrings\": {},\n    \"SecretArn\": {},\n    \"StatementName\": {},\n    \"Status\": {},\n    \"UpdatedAt\": {}\n  },\n  \"required\": [\n    \"Id\"\n  ],\n  \"description\": \"The SQL statement to run.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-statement-data-schema.json\",\n  \"title\": \"StatementData\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-statement-data-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: StatementData
---
