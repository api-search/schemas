---
description: Describes a security group.
layout: schema
name: ClusterSecurityGroup
properties_list:
- description: ''
  name: ClusterSecurityGroupName
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: EC2SecurityGroups
  type: object
- description: ''
  name: IPRanges
  type: object
- description: ''
  name: Tags
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-cluster-security-group-schema.json
slug: redshift-cluster-security-group
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterSecurityGroupName\": {},\n    \"Description\": {},\n    \"EC2SecurityGroups\": {},\n    \"IPRanges\": {},\n    \"Tags\": {}\n  },\n  \"description\": \"Describes a security group.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-security-group-schema.json\",\n  \"title\": \"ClusterSecurityGroup\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-security-group-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ClusterSecurityGroup
---
