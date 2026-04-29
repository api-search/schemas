---
description: Contains the output from the <a>DescribeClusterVersions</a> action.
layout: schema
name: ClusterVersionsMessage
properties_list:
- description: ''
  name: Marker
  type: object
- description: ''
  name: ClusterVersions
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-cluster-versions-message-schema.json
slug: redshift-cluster-versions-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Marker\": {},\n    \"ClusterVersions\": {}\n  },\n  \"description\": \"Contains the output from the <a>DescribeClusterVersions</a> action. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-versions-message-schema.json\",\n  \"title\": \"ClusterVersionsMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-versions-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ClusterVersionsMessage
---
