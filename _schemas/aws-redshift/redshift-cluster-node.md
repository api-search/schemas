---
description: The identifier of a node in a cluster.
layout: schema
name: ClusterNode
properties_list:
- description: ''
  name: NodeRole
  type: object
- description: ''
  name: PrivateIPAddress
  type: object
- description: ''
  name: PublicIPAddress
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-cluster-node-schema.json
slug: redshift-cluster-node
source_filename: redshift-cluster-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"NodeRole\": {},\n    \"PrivateIPAddress\": {},\n    \"PublicIPAddress\": {}\n  },\n  \"description\": \"The identifier of a node in a cluster.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-node-schema.json\",\n  \"title\": \"ClusterNode\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-node-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ClusterNode
---
