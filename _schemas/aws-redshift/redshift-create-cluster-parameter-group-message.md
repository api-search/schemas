---
description: <p/>
layout: schema
name: CreateClusterParameterGroupMessage
properties_list:
- description: ''
  name: ParameterGroupName
  type: object
- description: ''
  name: ParameterGroupFamily
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Tags
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-cluster-parameter-group-message-schema.json
slug: redshift-create-cluster-parameter-group-message
source_filename: redshift-create-cluster-parameter-group-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ParameterGroupName\": {},\n    \"ParameterGroupFamily\": {},\n    \"Description\": {},\n    \"Tags\": {}\n  },\n  \"required\": [\n    \"ParameterGroupName\",\n    \"ParameterGroupFamily\",\n    \"Description\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-cluster-parameter-group-message-schema.json\",\n  \"title\": \"CreateClusterParameterGroupMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-cluster-parameter-group-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateClusterParameterGroupMessage
---
