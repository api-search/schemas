---
description: DescribeDBClustersResponse schema from Neptune
layout: schema
name: DescribeDBClustersResponse
properties_list:
- description: ''
  name: DBClusters
  type: array
- description: ''
  name: Marker
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/management-describe-db-clusters-response-schema.json
slug: management-describe-db-clusters-response
source_filename: management-describe-db-clusters-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-describe-db-clusters-response-schema.json\",\n  \"title\": \"DescribeDBClustersResponse\",\n  \"description\": \"DescribeDBClustersResponse schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBClusters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DBCluster\"\n      }\n    },\n    \"Marker\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-describe-db-clusters-response-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: DescribeDBClustersResponse
---
