---
description: ClusterNodesList schema from Amazon Redshift
layout: schema
name: ClusterNodesList
properties_list: []
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-cluster-nodes-list-schema.json
slug: redshift-cluster-nodes-list
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"NodeRole\": {},\n      \"PrivateIPAddress\": {},\n      \"PublicIPAddress\": {}\n    },\n    \"description\": \"The identifier of a node in a cluster.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-nodes-list-schema.json\",\n  \"title\": \"ClusterNodesList\",\n  \"description\": \"ClusterNodesList schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-nodes-list-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ClusterNodesList
---
