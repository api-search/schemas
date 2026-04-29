---
description: ListTablesRequest schema from Amazon Redshift
layout: schema
name: ListTablesRequest
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: ConnectedDatabase
  type: object
- description: ''
  name: Database
  type: object
- description: ''
  name: DbUser
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: SchemaPattern
  type: object
- description: ''
  name: SecretArn
  type: object
- description: ''
  name: TablePattern
  type: object
- description: ''
  name: WorkgroupName
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-data-list-tables-request-schema.json
slug: redshift-data-list-tables-request
source_filename: redshift-data-list-tables-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"ConnectedDatabase\": {},\n    \"Database\": {},\n    \"DbUser\": {},\n    \"MaxResults\": {},\n    \"NextToken\": {},\n    \"SchemaPattern\": {},\n    \"SecretArn\": {},\n    \"TablePattern\": {},\n    \"WorkgroupName\": {}\n  },\n  \"required\": [\n    \"Database\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-list-tables-request-schema.json\",\n  \"title\": \"ListTablesRequest\",\n  \"description\": \"ListTablesRequest schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-list-tables-request-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ListTablesRequest
---
