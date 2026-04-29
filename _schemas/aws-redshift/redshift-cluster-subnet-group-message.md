---
description: Contains the output from the <a>DescribeClusterSubnetGroups</a> action.
layout: schema
name: ClusterSubnetGroupMessage
properties_list:
- description: ''
  name: Marker
  type: object
- description: ''
  name: ClusterSubnetGroups
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-cluster-subnet-group-message-schema.json
slug: redshift-cluster-subnet-group-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Marker\": {},\n    \"ClusterSubnetGroups\": {}\n  },\n  \"description\": \"Contains the output from the <a>DescribeClusterSubnetGroups</a> action. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-subnet-group-message-schema.json\",\n  \"title\": \"ClusterSubnetGroupMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-subnet-group-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ClusterSubnetGroupMessage
---
