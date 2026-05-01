---
description: Response from the DescribeDBClusters action
layout: schema
name: DescribeDBClustersResponse
properties_list:
- description: A list of DB cluster descriptions
  name: dBClusters
  type: array
- description: An optional pagination token provided by a previous request
  name: marker
  type: string
provider_name: Amazon RDS
provider_slug: amazon-rds
schema_file: json-schema/amazon-rds-openapi-describe-db-clusters-response-schema.json
slug: amazon-rds-openapi-describe-db-clusters-response
source_filename: amazon-rds-openapi-describe-db-clusters-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-describe-db-clusters-response-schema.json\",\n  \"title\": \"DescribeDBClustersResponse\",\n  \"description\": \"Response from the DescribeDBClusters action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dBClusters\": {\n      \"type\": \"array\",\n      \"description\": \"A list of DB cluster descriptions\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DBCluster\"\n      }\n    },\n    \"marker\": {\n      \"type\": \"string\",\n      \"description\": \"An optional pagination token provided by a previous request\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-describe-db-clusters-response-schema.json
tags:
- Cloud Databases
- Database Service
- DBaaS
- Managed Databases
- Relational Databases
title: DescribeDBClustersResponse
---
