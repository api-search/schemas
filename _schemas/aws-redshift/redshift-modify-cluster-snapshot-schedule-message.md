---
description: ModifyClusterSnapshotScheduleMessage schema from Amazon Redshift
layout: schema
name: ModifyClusterSnapshotScheduleMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: ScheduleIdentifier
  type: object
- description: ''
  name: DisassociateSchedule
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-cluster-snapshot-schedule-message-schema.json
slug: redshift-modify-cluster-snapshot-schedule-message
source_filename: redshift-modify-cluster-snapshot-schedule-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"ScheduleIdentifier\": {},\n    \"DisassociateSchedule\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-snapshot-schedule-message-schema.json\",\n  \"title\": \"ModifyClusterSnapshotScheduleMessage\",\n  \"description\": \"ModifyClusterSnapshotScheduleMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-snapshot-schedule-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifyClusterSnapshotScheduleMessage
---
