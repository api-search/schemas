---
description: Response from the DescribeDBInstances action
layout: schema
name: DescribeDBInstancesResponse
properties_list:
- description: A list of DB instance descriptions
  name: dBInstances
  type: array
- description: An optional pagination token provided by a previous request
  name: marker
  type: string
provider_name: Amazon RDS
provider_slug: amazon-rds
schema_file: json-schema/amazon-rds-openapi-describe-db-instances-response-schema.json
slug: amazon-rds-openapi-describe-db-instances-response
source_filename: amazon-rds-openapi-describe-db-instances-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-describe-db-instances-response-schema.json\",\n  \"title\": \"DescribeDBInstancesResponse\",\n  \"description\": \"Response from the DescribeDBInstances action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dBInstances\": {\n      \"type\": \"array\",\n      \"description\": \"A list of DB instance descriptions\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DBInstance\"\n      }\n    },\n    \"marker\": {\n      \"type\": \"string\",\n      \"description\": \"An optional pagination token provided by a previous request\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-describe-db-instances-response-schema.json
tags:
- AWS
- Cloud Databases
- Database Service
- DBaaS
- Managed Databases
- Relational Databases
title: DescribeDBInstancesResponse
---
