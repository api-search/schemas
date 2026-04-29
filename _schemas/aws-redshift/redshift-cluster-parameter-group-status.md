---
description: Describes the status of a parameter group.
layout: schema
name: ClusterParameterGroupStatus
properties_list:
- description: ''
  name: ParameterGroupName
  type: object
- description: ''
  name: ParameterApplyStatus
  type: object
- description: ''
  name: ClusterParameterStatusList
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-cluster-parameter-group-status-schema.json
slug: redshift-cluster-parameter-group-status
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ParameterGroupName\": {},\n    \"ParameterApplyStatus\": {},\n    \"ClusterParameterStatusList\": {}\n  },\n  \"description\": \"Describes the status of a parameter group.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-parameter-group-status-schema.json\",\n  \"title\": \"ClusterParameterGroupStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-parameter-group-status-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ClusterParameterGroupStatus
---
