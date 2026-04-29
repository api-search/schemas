---
description: <p/>
layout: schema
name: ModifyClusterIamRolesMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: AddIamRoles
  type: object
- description: ''
  name: RemoveIamRoles
  type: object
- description: ''
  name: DefaultIamRoleArn
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-cluster-iam-roles-message-schema.json
slug: redshift-modify-cluster-iam-roles-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"AddIamRoles\": {},\n    \"RemoveIamRoles\": {},\n    \"DefaultIamRoleArn\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-iam-roles-message-schema.json\",\n  \"title\": \"ModifyClusterIamRolesMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-iam-roles-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifyClusterIamRolesMessage
---
