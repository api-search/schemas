---
description: The request parameters to get cluster credentials.
layout: schema
name: GetClusterCredentialsMessage
properties_list:
- description: ''
  name: DbUser
  type: object
- description: ''
  name: DbName
  type: object
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: DurationSeconds
  type: object
- description: ''
  name: AutoCreate
  type: object
- description: ''
  name: DbGroups
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-get-cluster-credentials-message-schema.json
slug: redshift-get-cluster-credentials-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DbUser\": {},\n    \"DbName\": {},\n    \"ClusterIdentifier\": {},\n    \"DurationSeconds\": {},\n    \"AutoCreate\": {},\n    \"DbGroups\": {}\n  },\n  \"required\": [\n    \"DbUser\",\n    \"ClusterIdentifier\"\n  ],\n  \"description\": \"The request parameters to get cluster credentials.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-get-cluster-credentials-message-schema.json\",\n  \"title\": \"GetClusterCredentialsMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-get-cluster-credentials-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: GetClusterCredentialsMessage
---
