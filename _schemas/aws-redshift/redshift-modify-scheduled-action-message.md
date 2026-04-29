---
description: ModifyScheduledActionMessage schema from Amazon Redshift
layout: schema
name: ModifyScheduledActionMessage
properties_list:
- description: ''
  name: ScheduledActionName
  type: object
- description: ''
  name: TargetAction
  type: object
- description: ''
  name: Schedule
  type: object
- description: ''
  name: IamRole
  type: object
- description: ''
  name: ScheduledActionDescription
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: Enable
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-scheduled-action-message-schema.json
slug: redshift-modify-scheduled-action-message
source_filename: redshift-modify-scheduled-action-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScheduledActionName\": {},\n    \"TargetAction\": {},\n    \"Schedule\": {},\n    \"IamRole\": {},\n    \"ScheduledActionDescription\": {},\n    \"StartTime\": {},\n    \"EndTime\": {},\n    \"Enable\": {}\n  },\n  \"required\": [\n    \"ScheduledActionName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-scheduled-action-message-schema.json\",\n  \"title\": \"ModifyScheduledActionMessage\",\n  \"description\": \"ModifyScheduledActionMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-scheduled-action-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifyScheduledActionMessage
---
