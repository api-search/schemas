---
description: <p/>
layout: schema
name: ResetClusterParameterGroupMessage
properties_list:
- description: ''
  name: ParameterGroupName
  type: object
- description: ''
  name: ResetAllParameters
  type: object
- description: ''
  name: Parameters
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-reset-cluster-parameter-group-message-schema.json
slug: redshift-reset-cluster-parameter-group-message
source_filename: redshift-reset-cluster-parameter-group-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ParameterGroupName\": {},\n    \"ResetAllParameters\": {},\n    \"Parameters\": {}\n  },\n  \"required\": [\n    \"ParameterGroupName\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-reset-cluster-parameter-group-message-schema.json\",\n  \"title\": \"ResetClusterParameterGroupMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-reset-cluster-parameter-group-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ResetClusterParameterGroupMessage
---
