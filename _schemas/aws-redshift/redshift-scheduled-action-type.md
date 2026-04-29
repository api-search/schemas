---
description: The action type that specifies an Amazon Redshift API operation that is supported by the Amazon Redshift scheduler.
layout: schema
name: ScheduledActionType
properties_list:
- description: ''
  name: ResizeCluster
  type: object
- description: ''
  name: PauseCluster
  type: object
- description: ''
  name: ResumeCluster
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-scheduled-action-type-schema.json
slug: redshift-scheduled-action-type
source_filename: redshift-scheduled-action-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResizeCluster\": {},\n    \"PauseCluster\": {},\n    \"ResumeCluster\": {}\n  },\n  \"description\": \"The action type that specifies an Amazon Redshift API operation that is supported by the Amazon Redshift scheduler. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-scheduled-action-type-schema.json\",\n  \"title\": \"ScheduledActionType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-scheduled-action-type-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ScheduledActionType
---
