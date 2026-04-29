---
description: CreateClusterParameterGroupResult schema from Amazon Redshift
layout: schema
name: CreateClusterParameterGroupResult
properties_list:
- description: Describes a parameter group.
  name: ClusterParameterGroup
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-cluster-parameter-group-result-schema.json
slug: redshift-create-cluster-parameter-group-result
source_filename: redshift-create-cluster-parameter-group-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterParameterGroup\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ParameterGroupName\": {},\n        \"ParameterGroupFamily\": {},\n        \"Description\": {},\n        \"Tags\": {}\n      },\n      \"description\": \"Describes a parameter group.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-cluster-parameter-group-result-schema.json\",\n  \"title\": \"CreateClusterParameterGroupResult\",\n  \"description\": \"CreateClusterParameterGroupResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-cluster-parameter-group-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateClusterParameterGroupResult
---
