---
description: Describes a modify cluster parameter group operation.
layout: schema
name: ModifyClusterParameterGroupMessage
properties_list:
- description: ''
  name: ParameterGroupName
  type: object
- description: ''
  name: Parameters
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-cluster-parameter-group-message-schema.json
slug: redshift-modify-cluster-parameter-group-message
source_filename: redshift-modify-cluster-parameter-group-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ParameterGroupName\": {},\n    \"Parameters\": {}\n  },\n  \"required\": [\n    \"ParameterGroupName\",\n    \"Parameters\"\n  ],\n  \"description\": \"Describes a modify cluster parameter group operation. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-parameter-group-message-schema.json\",\n  \"title\": \"ModifyClusterParameterGroupMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-parameter-group-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifyClusterParameterGroupMessage
---
