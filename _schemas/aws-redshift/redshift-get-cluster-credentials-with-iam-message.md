---
description: GetClusterCredentialsWithIAMMessage schema from Amazon Redshift
layout: schema
name: GetClusterCredentialsWithIAMMessage
properties_list:
- description: ''
  name: DbName
  type: object
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: DurationSeconds
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-get-cluster-credentials-with-iam-message-schema.json
slug: redshift-get-cluster-credentials-with-iam-message
source_filename: redshift-get-cluster-credentials-with-iam-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DbName\": {},\n    \"ClusterIdentifier\": {},\n    \"DurationSeconds\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-get-cluster-credentials-with-iam-message-schema.json\",\n  \"title\": \"GetClusterCredentialsWithIAMMessage\",\n  \"description\": \"GetClusterCredentialsWithIAMMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-get-cluster-credentials-with-iam-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: GetClusterCredentialsWithIAMMessage
---
