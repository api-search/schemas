---
description: CreateClusterSecurityGroupResult schema from Amazon Redshift
layout: schema
name: CreateClusterSecurityGroupResult
properties_list:
- description: Describes a security group.
  name: ClusterSecurityGroup
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-cluster-security-group-result-schema.json
slug: redshift-create-cluster-security-group-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterSecurityGroup\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ClusterSecurityGroupName\": {},\n        \"Description\": {},\n        \"EC2SecurityGroups\": {},\n        \"IPRanges\": {},\n        \"Tags\": {}\n      },\n      \"description\": \"Describes a security group.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-cluster-security-group-result-schema.json\",\n  \"title\": \"CreateClusterSecurityGroupResult\",\n  \"description\": \"CreateClusterSecurityGroupResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-cluster-security-group-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateClusterSecurityGroupResult
---
