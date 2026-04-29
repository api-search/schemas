---
description: DescribeNodeConfigurationOptionsMessage schema from Amazon Redshift
layout: schema
name: DescribeNodeConfigurationOptionsMessage
properties_list:
- description: ''
  name: ActionType
  type: object
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: SnapshotIdentifier
  type: object
- description: ''
  name: SnapshotArn
  type: object
- description: ''
  name: OwnerAccount
  type: object
- description: ''
  name: Filters
  type: object
- description: ''
  name: Marker
  type: object
- description: ''
  name: MaxRecords
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-describe-node-configuration-options-message-schema.json
slug: redshift-describe-node-configuration-options-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActionType\": {},\n    \"ClusterIdentifier\": {},\n    \"SnapshotIdentifier\": {},\n    \"SnapshotArn\": {},\n    \"OwnerAccount\": {},\n    \"Filters\": {},\n    \"Marker\": {},\n    \"MaxRecords\": {}\n  },\n  \"required\": [\n    \"ActionType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-describe-node-configuration-options-message-schema.json\",\n  \"title\": \"DescribeNodeConfigurationOptionsMessage\",\n  \"description\": \"DescribeNodeConfigurationOptionsMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-describe-node-configuration-options-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: DescribeNodeConfigurationOptionsMessage
---
