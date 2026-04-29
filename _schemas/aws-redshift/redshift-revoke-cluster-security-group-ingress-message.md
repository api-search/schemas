---
description: <p/>
layout: schema
name: RevokeClusterSecurityGroupIngressMessage
properties_list:
- description: ''
  name: ClusterSecurityGroupName
  type: object
- description: ''
  name: CIDRIP
  type: object
- description: ''
  name: EC2SecurityGroupName
  type: object
- description: ''
  name: EC2SecurityGroupOwnerId
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-revoke-cluster-security-group-ingress-message-schema.json
slug: redshift-revoke-cluster-security-group-ingress-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterSecurityGroupName\": {},\n    \"CIDRIP\": {},\n    \"EC2SecurityGroupName\": {},\n    \"EC2SecurityGroupOwnerId\": {}\n  },\n  \"required\": [\n    \"ClusterSecurityGroupName\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-revoke-cluster-security-group-ingress-message-schema.json\",\n  \"title\": \"RevokeClusterSecurityGroupIngressMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-revoke-cluster-security-group-ingress-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: RevokeClusterSecurityGroupIngressMessage
---
