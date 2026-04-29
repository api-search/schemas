---
description: Describes a subnet group.
layout: schema
name: ClusterSubnetGroup
properties_list:
- description: ''
  name: ClusterSubnetGroupName
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: SubnetGroupStatus
  type: object
- description: ''
  name: Subnets
  type: object
- description: ''
  name: Tags
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-cluster-subnet-group-schema.json
slug: redshift-cluster-subnet-group
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterSubnetGroupName\": {},\n    \"Description\": {},\n    \"VpcId\": {},\n    \"SubnetGroupStatus\": {},\n    \"Subnets\": {},\n    \"Tags\": {}\n  },\n  \"description\": \"Describes a subnet group.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-subnet-group-schema.json\",\n  \"title\": \"ClusterSubnetGroup\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-subnet-group-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ClusterSubnetGroup
---
