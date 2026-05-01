---
description: Contains the details of a Neptune DB subnet group.
layout: schema
name: DBSubnetGroup
properties_list:
- description: ''
  name: DBSubnetGroupName
  type: string
- description: ''
  name: DBSubnetGroupDescription
  type: string
- description: ''
  name: VpcId
  type: string
- description: ''
  name: SubnetGroupStatus
  type: string
- description: ''
  name: Subnets
  type: array
- description: ''
  name: DBSubnetGroupArn
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/management-db-subnet-group-schema.json
slug: management-db-subnet-group
source_filename: management-db-subnet-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-db-subnet-group-schema.json\",\n  \"title\": \"DBSubnetGroup\",\n  \"description\": \"Contains the details of a Neptune DB subnet group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBSubnetGroupName\": {\n      \"type\": \"string\"\n    },\n    \"DBSubnetGroupDescription\": {\n      \"type\": \"string\"\n    },\n    \"VpcId\": {\n      \"type\": \"string\"\n    },\n    \"SubnetGroupStatus\": {\n      \"type\": \"string\"\n    },\n    \"Subnets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"SubnetIdentifier\": {\n            \"type\": \"string\"\n          },\n          \"SubnetAvailabilityZone\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Name\": {\n             \
  \   \"type\": \"string\"\n              }\n            }\n          },\n          \"SubnetStatus\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"DBSubnetGroupArn\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-db-subnet-group-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: DBSubnetGroup
---
