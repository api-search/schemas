---
description: ModifySnapshotScheduleMessage schema from Amazon Redshift
layout: schema
name: ModifySnapshotScheduleMessage
properties_list:
- description: ''
  name: ScheduleIdentifier
  type: object
- description: ''
  name: ScheduleDefinitions
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-snapshot-schedule-message-schema.json
slug: redshift-modify-snapshot-schedule-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScheduleIdentifier\": {},\n    \"ScheduleDefinitions\": {}\n  },\n  \"required\": [\n    \"ScheduleIdentifier\",\n    \"ScheduleDefinitions\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-snapshot-schedule-message-schema.json\",\n  \"title\": \"ModifySnapshotScheduleMessage\",\n  \"description\": \"ModifySnapshotScheduleMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-snapshot-schedule-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifySnapshotScheduleMessage
---
