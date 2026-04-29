---
description: <p/>
layout: schema
name: DescribeClusterParametersMessage
properties_list:
- description: ''
  name: ParameterGroupName
  type: object
- description: ''
  name: Source
  type: object
- description: ''
  name: MaxRecords
  type: object
- description: ''
  name: Marker
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-describe-cluster-parameters-message-schema.json
slug: redshift-describe-cluster-parameters-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ParameterGroupName\": {},\n    \"Source\": {},\n    \"MaxRecords\": {},\n    \"Marker\": {}\n  },\n  \"required\": [\n    \"ParameterGroupName\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-describe-cluster-parameters-message-schema.json\",\n  \"title\": \"DescribeClusterParametersMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-describe-cluster-parameters-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: DescribeClusterParametersMessage
---
