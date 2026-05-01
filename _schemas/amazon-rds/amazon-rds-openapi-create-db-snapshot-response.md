---
description: Response from the CreateDBSnapshot action
layout: schema
name: CreateDBSnapshotResponse
properties_list:
- description: ''
  name: dBSnapshot
  type: object
provider_name: Amazon RDS
provider_slug: amazon-rds
schema_file: json-schema/amazon-rds-openapi-create-db-snapshot-response-schema.json
slug: amazon-rds-openapi-create-db-snapshot-response
source_filename: amazon-rds-openapi-create-db-snapshot-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-create-db-snapshot-response-schema.json\",\n  \"title\": \"CreateDBSnapshotResponse\",\n  \"description\": \"Response from the CreateDBSnapshot action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dBSnapshot\": {\n      \"$ref\": \"#/components/schemas/DBSnapshot\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-create-db-snapshot-response-schema.json
tags:
- Cloud Databases
- Database Service
- DBaaS
- Managed Databases
- Relational Databases
title: CreateDBSnapshotResponse
---
