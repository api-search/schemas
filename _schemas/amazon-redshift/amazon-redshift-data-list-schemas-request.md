---
description: ''
layout: schema
name: ListSchemasRequest
properties_list:
- description: The cluster identifier
  name: ClusterIdentifier
  type: string
- description: The name of the database containing the schemas
  name: Database
  type: string
- description: The database user for temporary credentials
  name: DbUser
  type: string
- description: ARN of the secret in Secrets Manager
  name: SecretArn
  type: string
- description: The serverless workgroup name
  name: WorkgroupName
  type: string
- description: A pattern to filter schemas. Uses SQL LIKE syntax where underscore matches one character and percent matches zero or more characters.
  name: SchemaPattern
  type: string
- description: Maximum number of schemas to return
  name: MaxResults
  type: integer
- description: Pagination token for the next page
  name: NextToken
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-list-schemas-request-schema.json
slug: amazon-redshift-data-list-schemas-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListSchemasRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The cluster identifier\"\n    },\n    \"Database\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database containing the schemas\"\n    },\n    \"DbUser\": {\n      \"type\": \"string\",\n      \"description\": \"The database user for temporary credentials\"\n    },\n    \"SecretArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the secret in Secrets Manager\"\n    },\n    \"WorkgroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The serverless workgroup name\"\n    },\n    \"SchemaPattern\": {\n      \"type\": \"string\",\n      \"description\": \"A pattern to filter schemas. Uses SQL LIKE syntax where underscore matches one character and percent matches zero or more characters.\"\
  \n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of schemas to return\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token for the next page\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-list-schemas-request-schema.json
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
title: ListSchemasRequest
---
