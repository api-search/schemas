---
description: ModifyClusterSubnetGroupResult schema from Amazon Redshift
layout: schema
name: ModifyClusterSubnetGroupResult
properties_list:
- description: Describes a subnet group.
  name: ClusterSubnetGroup
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-cluster-subnet-group-result-schema.json
slug: redshift-modify-cluster-subnet-group-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterSubnetGroup\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ClusterSubnetGroupName\": {},\n        \"Description\": {},\n        \"VpcId\": {},\n        \"SubnetGroupStatus\": {},\n        \"Subnets\": {},\n        \"Tags\": {}\n      },\n      \"description\": \"Describes a subnet group.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-subnet-group-result-schema.json\",\n  \"title\": \"ModifyClusterSubnetGroupResult\",\n  \"description\": \"ModifyClusterSubnetGroupResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-subnet-group-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifyClusterSubnetGroupResult
---
