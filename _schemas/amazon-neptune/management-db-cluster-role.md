---
description: An IAM role associated with a Neptune DB cluster.
layout: schema
name: DBClusterRole
properties_list:
- description: The ARN of the IAM role.
  name: RoleArn
  type: string
- description: The status of the association (active, pending, error).
  name: Status
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/management-db-cluster-role-schema.json
slug: management-db-cluster-role
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-db-cluster-role-schema.json\",\n  \"title\": \"DBClusterRole\",\n  \"description\": \"An IAM role associated with a Neptune DB cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the IAM role.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the association (active, pending, error).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-db-cluster-role-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: DBClusterRole
---
