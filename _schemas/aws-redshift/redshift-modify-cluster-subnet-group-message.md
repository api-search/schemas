---
description: <p/>
layout: schema
name: ModifyClusterSubnetGroupMessage
properties_list:
- description: ''
  name: ClusterSubnetGroupName
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: SubnetIds
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-cluster-subnet-group-message-schema.json
slug: redshift-modify-cluster-subnet-group-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterSubnetGroupName\": {},\n    \"Description\": {},\n    \"SubnetIds\": {}\n  },\n  \"required\": [\n    \"ClusterSubnetGroupName\",\n    \"SubnetIds\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-subnet-group-message-schema.json\",\n  \"title\": \"ModifyClusterSubnetGroupMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-subnet-group-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifyClusterSubnetGroupMessage
---
