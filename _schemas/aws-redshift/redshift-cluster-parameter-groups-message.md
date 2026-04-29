---
description: Contains the output from the <a>DescribeClusterParameterGroups</a> action.
layout: schema
name: ClusterParameterGroupsMessage
properties_list:
- description: ''
  name: Marker
  type: object
- description: ''
  name: ParameterGroups
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-cluster-parameter-groups-message-schema.json
slug: redshift-cluster-parameter-groups-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Marker\": {},\n    \"ParameterGroups\": {}\n  },\n  \"description\": \"Contains the output from the <a>DescribeClusterParameterGroups</a> action. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-parameter-groups-message-schema.json\",\n  \"title\": \"ClusterParameterGroupsMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-parameter-groups-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ClusterParameterGroupsMessage
---
