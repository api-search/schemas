---
description: DescribeSnapshotSchedulesMessage schema from Amazon Redshift
layout: schema
name: DescribeSnapshotSchedulesMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: ScheduleIdentifier
  type: object
- description: ''
  name: TagKeys
  type: object
- description: ''
  name: TagValues
  type: object
- description: ''
  name: Marker
  type: object
- description: ''
  name: MaxRecords
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-describe-snapshot-schedules-message-schema.json
slug: redshift-describe-snapshot-schedules-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"ScheduleIdentifier\": {},\n    \"TagKeys\": {},\n    \"TagValues\": {},\n    \"Marker\": {},\n    \"MaxRecords\": {}\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-describe-snapshot-schedules-message-schema.json\",\n  \"title\": \"DescribeSnapshotSchedulesMessage\",\n  \"description\": \"DescribeSnapshotSchedulesMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-describe-snapshot-schedules-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: DescribeSnapshotSchedulesMessage
---
