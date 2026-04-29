---
description: DescribeDefaultClusterParametersResult schema from Amazon Redshift
layout: schema
name: DescribeDefaultClusterParametersResult
properties_list:
- description: Describes the default cluster parameters for a parameter group family.
  name: DefaultClusterParameters
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-describe-default-cluster-parameters-result-schema.json
slug: redshift-describe-default-cluster-parameters-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DefaultClusterParameters\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ParameterGroupFamily\": {},\n        \"Marker\": {},\n        \"Parameters\": {}\n      },\n      \"description\": \"Describes the default cluster parameters for a parameter group family.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-describe-default-cluster-parameters-result-schema.json\",\n  \"title\": \"DescribeDefaultClusterParametersResult\",\n  \"description\": \"DescribeDefaultClusterParametersResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-describe-default-cluster-parameters-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: DescribeDefaultClusterParametersResult
---
