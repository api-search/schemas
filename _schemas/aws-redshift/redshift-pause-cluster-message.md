---
description: Describes a pause cluster operation. For example, a scheduled action to run the <code>PauseCluster</code> API operation.
layout: schema
name: PauseClusterMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-pause-cluster-message-schema.json
slug: redshift-pause-cluster-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\"\n  ],\n  \"description\": \"Describes a pause cluster operation. For example, a scheduled action to run the <code>PauseCluster</code> API operation. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-pause-cluster-message-schema.json\",\n  \"title\": \"PauseClusterMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-pause-cluster-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: PauseClusterMessage
---
