---
description: ''
layout: schema
name: CollectiveCluster
properties_list:
- description: Cluster name
  name: name
  type: string
- description: Cluster description
  name: description
  type: string
- description: Number of members in the cluster
  name: memberCount
  type: integer
- description: Number of started members
  name: membersStarted
  type: integer
- description: List of member server names
  name: members
  type: array
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-collective-controller-rest-collective-cluster-schema.json
slug: websphere-liberty-collective-controller-rest-collective-cluster
source_filename: websphere-liberty-collective-controller-rest-collective-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CollectiveCluster\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster description\"\n    },\n    \"memberCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of members in the cluster\"\n    },\n    \"membersStarted\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of started members\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"List of member server names\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-collective-controller-rest-collective-cluster-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: CollectiveCluster
---
