---
description: Describes a cluster version, including the parameter group family and description of the version.
layout: schema
name: ClusterVersion
properties_list:
- description: ''
  name: ClusterVersion
  type: object
- description: ''
  name: ClusterParameterGroupFamily
  type: object
- description: ''
  name: Description
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-cluster-version-schema.json
slug: redshift-cluster-version
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterVersion\": {},\n    \"ClusterParameterGroupFamily\": {},\n    \"Description\": {}\n  },\n  \"description\": \"Describes a cluster version, including the parameter group family and description of the version.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-version-schema.json\",\n  \"title\": \"ClusterVersion\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-version-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ClusterVersion
---
