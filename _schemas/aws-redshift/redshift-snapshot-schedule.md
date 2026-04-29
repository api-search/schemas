---
description: Describes a snapshot schedule. You can set a regular interval for creating snapshots of a cluster. You can also schedule snapshots for specific dates.
layout: schema
name: SnapshotSchedule
properties_list:
- description: ''
  name: ScheduleDefinitions
  type: object
- description: ''
  name: ScheduleIdentifier
  type: object
- description: ''
  name: ScheduleDescription
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: NextInvocations
  type: object
- description: ''
  name: AssociatedClusterCount
  type: object
- description: ''
  name: AssociatedClusters
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-snapshot-schedule-schema.json
slug: redshift-snapshot-schedule
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScheduleDefinitions\": {},\n    \"ScheduleIdentifier\": {},\n    \"ScheduleDescription\": {},\n    \"Tags\": {},\n    \"NextInvocations\": {},\n    \"AssociatedClusterCount\": {},\n    \"AssociatedClusters\": {}\n  },\n  \"description\": \"Describes a snapshot schedule. You can set a regular interval for creating snapshots of a cluster. You can also schedule snapshots for specific dates. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-snapshot-schedule-schema.json\",\n  \"title\": \"SnapshotSchedule\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-snapshot-schedule-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: SnapshotSchedule
---
