---
description: CreateClusterSubnetGroupResult schema from Amazon Redshift
layout: schema
name: CreateClusterSubnetGroupResult
properties_list:
- description: Describes a subnet group.
  name: ClusterSubnetGroup
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-cluster-subnet-group-result-schema.json
slug: redshift-create-cluster-subnet-group-result
source_filename: redshift-create-cluster-subnet-group-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterSubnetGroup\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ClusterSubnetGroupName\": {},\n        \"Description\": {},\n        \"VpcId\": {},\n        \"SubnetGroupStatus\": {},\n        \"Subnets\": {},\n        \"Tags\": {}\n      },\n      \"description\": \"Describes a subnet group.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-cluster-subnet-group-result-schema.json\",\n  \"title\": \"CreateClusterSubnetGroupResult\",\n  \"description\": \"CreateClusterSubnetGroupResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-cluster-subnet-group-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateClusterSubnetGroupResult
---
