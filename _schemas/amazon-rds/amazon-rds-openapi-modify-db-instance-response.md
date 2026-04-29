---
description: Response from the ModifyDBInstance action
layout: schema
name: ModifyDBInstanceResponse
properties_list:
- description: ''
  name: dBInstance
  type: object
provider_name: Amazon RDS
provider_slug: amazon-rds
schema_file: json-schema/amazon-rds-openapi-modify-db-instance-response-schema.json
slug: amazon-rds-openapi-modify-db-instance-response
source_filename: amazon-rds-openapi-modify-db-instance-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-modify-db-instance-response-schema.json\",\n  \"title\": \"ModifyDBInstanceResponse\",\n  \"description\": \"Response from the ModifyDBInstance action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dBInstance\": {\n      \"$ref\": \"#/components/schemas/DBInstance\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-modify-db-instance-response-schema.json
tags:
- AWS
- Cloud Databases
- Database Service
- DBaaS
- Managed Databases
- Relational Databases
title: ModifyDBInstanceResponse
---
