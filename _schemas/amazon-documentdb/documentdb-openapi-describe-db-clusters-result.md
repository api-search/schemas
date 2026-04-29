---
description: DescribeDBClustersResult schema from Amazon DocumentDB API
layout: schema
name: DescribeDBClustersResult
properties_list:
- description: ''
  name: DBClusters
  type: array
- description: ''
  name: Marker
  type: string
provider_name: Amazon DocumentDB
provider_slug: amazon-documentdb
schema_file: json-schema/documentdb-openapi-describe-db-clusters-result-schema.json
slug: documentdb-openapi-describe-db-clusters-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-documentdb/refs/heads/main/json-schema/documentdb-openapi-describe-db-clusters-result-schema.json\",\n  \"title\": \"DescribeDBClustersResult\",\n  \"description\": \"DescribeDBClustersResult schema from Amazon DocumentDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBClusters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DBCluster\"\n      }\n    },\n    \"Marker\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-documentdb/refs/heads/main/json-schema/documentdb-openapi-describe-db-clusters-result-schema.json
tags:
- Amazon Web Services
- AWS
- Database
- Document Database
- DocumentDB
- Managed Database
- MongoDB
- NoSQL
title: DescribeDBClustersResult
---
