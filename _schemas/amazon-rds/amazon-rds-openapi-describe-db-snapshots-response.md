---
description: Response from the DescribeDBSnapshots action
layout: schema
name: DescribeDBSnapshotsResponse
properties_list:
- description: A list of DB snapshot descriptions
  name: dBSnapshots
  type: array
- description: An optional pagination token provided by a previous request
  name: marker
  type: string
provider_name: Amazon RDS
provider_slug: amazon-rds
schema_file: json-schema/amazon-rds-openapi-describe-db-snapshots-response-schema.json
slug: amazon-rds-openapi-describe-db-snapshots-response
source_filename: amazon-rds-openapi-describe-db-snapshots-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-describe-db-snapshots-response-schema.json\",\n  \"title\": \"DescribeDBSnapshotsResponse\",\n  \"description\": \"Response from the DescribeDBSnapshots action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dBSnapshots\": {\n      \"type\": \"array\",\n      \"description\": \"A list of DB snapshot descriptions\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DBSnapshot\"\n      }\n    },\n    \"marker\": {\n      \"type\": \"string\",\n      \"description\": \"An optional pagination token provided by a previous request\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-describe-db-snapshots-response-schema.json
tags:
- AWS
- Cloud Databases
- Database Service
- DBaaS
- Managed Databases
- Relational Databases
title: DescribeDBSnapshotsResponse
---
