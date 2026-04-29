---
description: DescribeStatementResponse schema from Amazon Redshift
layout: schema
name: DescribeStatementResponse
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: Database
  type: object
- description: ''
  name: DbUser
  type: object
- description: ''
  name: Duration
  type: object
- description: ''
  name: Error
  type: object
- description: ''
  name: HasResultSet
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: QueryParameters
  type: object
- description: ''
  name: QueryString
  type: object
- description: ''
  name: RedshiftPid
  type: object
- description: ''
  name: RedshiftQueryId
  type: object
- description: ''
  name: ResultRows
  type: object
- description: ''
  name: ResultSize
  type: object
- description: ''
  name: SecretArn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: SubStatements
  type: object
- description: ''
  name: UpdatedAt
  type: object
- description: ''
  name: WorkgroupName
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-data-describe-statement-response-schema.json
slug: redshift-data-describe-statement-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"CreatedAt\": {},\n    \"Database\": {},\n    \"DbUser\": {},\n    \"Duration\": {},\n    \"Error\": {},\n    \"HasResultSet\": {},\n    \"Id\": {},\n    \"QueryParameters\": {},\n    \"QueryString\": {},\n    \"RedshiftPid\": {},\n    \"RedshiftQueryId\": {},\n    \"ResultRows\": {},\n    \"ResultSize\": {},\n    \"SecretArn\": {},\n    \"Status\": {},\n    \"SubStatements\": {},\n    \"UpdatedAt\": {},\n    \"WorkgroupName\": {}\n  },\n  \"required\": [\n    \"Id\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-describe-statement-response-schema.json\",\n  \"title\": \"DescribeStatementResponse\",\n  \"description\": \"DescribeStatementResponse schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-describe-statement-response-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: DescribeStatementResponse
---
