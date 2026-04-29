---
description: DescribeDBClusterSnapshotsResponse schema from Neptune
layout: schema
name: DescribeDBClusterSnapshotsResponse
properties_list:
- description: ''
  name: DBClusterSnapshots
  type: array
- description: ''
  name: Marker
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/management-describe-db-cluster-snapshots-response-schema.json
slug: management-describe-db-cluster-snapshots-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-describe-db-cluster-snapshots-response-schema.json\",\n  \"title\": \"DescribeDBClusterSnapshotsResponse\",\n  \"description\": \"DescribeDBClusterSnapshotsResponse schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBClusterSnapshots\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DBClusterSnapshot\"\n      }\n    },\n    \"Marker\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-describe-db-cluster-snapshots-response-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: DescribeDBClusterSnapshotsResponse
---
