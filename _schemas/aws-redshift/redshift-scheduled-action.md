---
description: Describes a scheduled action. You can use a scheduled action to trigger some Amazon Redshift API operations on a schedule. For information about which API operations can be scheduled, see <a>ScheduledActionType</a>.
layout: schema
name: ScheduledAction
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
  name: State
  type: object
- description: ''
  name: NextInvocations
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-scheduled-action-schema.json
slug: redshift-scheduled-action
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ScheduledAction
---
