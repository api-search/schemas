---
description: BatchExecuteStatementInput schema from Amazon Redshift
layout: schema
name: BatchExecuteStatementInput
properties_list:
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: Database
  type: object
- description: ''
  name: DbUser
  type: object
- description: ''
  name: SecretArn
  type: object
- description: ''
  name: Sqls
  type: object
- description: ''
  name: StatementName
  type: object
- description: ''
  name: WithEvent
  type: object
- description: ''
  name: WorkgroupName
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-data-batch-execute-statement-input-schema.json
slug: redshift-data-batch-execute-statement-input
source_filename: redshift-data-batch-execute-statement-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientToken\": {},\n    \"ClusterIdentifier\": {},\n    \"Database\": {},\n    \"DbUser\": {},\n    \"SecretArn\": {},\n    \"Sqls\": {},\n    \"StatementName\": {},\n    \"WithEvent\": {},\n    \"WorkgroupName\": {}\n  },\n  \"required\": [\n    \"Database\",\n    \"Sqls\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-batch-execute-statement-input-schema.json\",\n  \"title\": \"BatchExecuteStatementInput\",\n  \"description\": \"BatchExecuteStatementInput schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-batch-execute-statement-input-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: BatchExecuteStatementInput
---
