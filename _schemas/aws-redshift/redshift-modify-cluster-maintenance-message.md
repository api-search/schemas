---
description: ModifyClusterMaintenanceMessage schema from Amazon Redshift
layout: schema
name: ModifyClusterMaintenanceMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: DeferMaintenance
  type: object
- description: ''
  name: DeferMaintenanceIdentifier
  type: object
- description: ''
  name: DeferMaintenanceStartTime
  type: object
- description: ''
  name: DeferMaintenanceEndTime
  type: object
- description: ''
  name: DeferMaintenanceDuration
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-cluster-maintenance-message-schema.json
slug: redshift-modify-cluster-maintenance-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"DeferMaintenance\": {},\n    \"DeferMaintenanceIdentifier\": {},\n    \"DeferMaintenanceStartTime\": {},\n    \"DeferMaintenanceEndTime\": {},\n    \"DeferMaintenanceDuration\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-maintenance-message-schema.json\",\n  \"title\": \"ModifyClusterMaintenanceMessage\",\n  \"description\": \"ModifyClusterMaintenanceMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-maintenance-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifyClusterMaintenanceMessage
---
