---
description: An Identity and Access Management (IAM) role that can be used by the associated Amazon Redshift cluster to access other Amazon Web Services services.
layout: schema
name: ClusterIamRole
properties_list:
- description: ''
  name: IamRoleArn
  type: object
- description: ''
  name: ApplyStatus
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-cluster-iam-role-schema.json
slug: redshift-cluster-iam-role
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IamRoleArn\": {},\n    \"ApplyStatus\": {}\n  },\n  \"description\": \"An Identity and Access Management (IAM) role that can be used by the associated Amazon Redshift cluster to access other Amazon Web Services services.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-iam-role-schema.json\",\n  \"title\": \"ClusterIamRole\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-iam-role-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ClusterIamRole
---
