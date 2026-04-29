---
description: AuthorizeClusterSecurityGroupIngressResult schema from Amazon Redshift
layout: schema
name: AuthorizeClusterSecurityGroupIngressResult
properties_list:
- description: Describes a security group.
  name: ClusterSecurityGroup
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-authorize-cluster-security-group-ingress-result-schema.json
slug: redshift-authorize-cluster-security-group-ingress-result
source_filename: redshift-authorize-cluster-security-group-ingress-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterSecurityGroup\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ClusterSecurityGroupName\": {},\n        \"Description\": {},\n        \"EC2SecurityGroups\": {},\n        \"IPRanges\": {},\n        \"Tags\": {}\n      },\n      \"description\": \"Describes a security group.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-authorize-cluster-security-group-ingress-result-schema.json\",\n  \"title\": \"AuthorizeClusterSecurityGroupIngressResult\",\n  \"description\": \"AuthorizeClusterSecurityGroupIngressResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-authorize-cluster-security-group-ingress-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: AuthorizeClusterSecurityGroupIngressResult
---
