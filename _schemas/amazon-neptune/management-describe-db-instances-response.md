---
description: DescribeDBInstancesResponse schema from Neptune
layout: schema
name: DescribeDBInstancesResponse
properties_list:
- description: ''
  name: DBInstances
  type: array
- description: ''
  name: Marker
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/management-describe-db-instances-response-schema.json
slug: management-describe-db-instances-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-describe-db-instances-response-schema.json\",\n  \"title\": \"DescribeDBInstancesResponse\",\n  \"description\": \"DescribeDBInstancesResponse schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBInstances\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DBInstance\"\n      }\n    },\n    \"Marker\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-describe-db-instances-response-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: DescribeDBInstancesResponse
---
