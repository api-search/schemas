---
description: ''
layout: schema
name: DescribeAlarmsInput
properties_list:
- description: The names of the alarms to retrieve information about.
  name: AlarmNames
  type: array
- description: An alarm name prefix. If specified, only alarms with names that start with this prefix are returned.
  name: AlarmNamePrefix
  type: string
- description: Specify this parameter to receive information only about alarms of the specified types.
  name: AlarmTypes
  type: array
- description: If you use this parameter and specify the name of a composite alarm, the operation returns information about the child alarms.
  name: ChildrenOfAlarmName
  type: string
- description: If you use this parameter and specify the name of a metric alarm, the operation returns information about the composite alarms that reference it.
  name: ParentsOfAlarmName
  type: string
- description: Use this parameter to filter the results to only those alarms that use a certain alarm action.
  name: ActionPrefix
  type: string
- description: The maximum number of alarm descriptions to retrieve.
  name: MaxRecords
  type: integer
- description: The token returned by a previous call to indicate there is more data available.
  name: NextToken
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-describe-alarms-input-schema.json
slug: cloudwatch-describe-alarms-input
source_filename: cloudwatch-describe-alarms-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeAlarmsInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlarmNames\": {\n      \"type\": \"array\",\n      \"description\": \"The names of the alarms to retrieve information about.\"\n    },\n    \"AlarmNamePrefix\": {\n      \"type\": \"string\",\n      \"description\": \"An alarm name prefix. If specified, only alarms with names that start with this prefix are returned.\"\n    },\n    \"AlarmTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Specify this parameter to receive information only about alarms of the specified types.\"\n    },\n    \"ChildrenOfAlarmName\": {\n      \"type\": \"string\",\n      \"description\": \"If you use this parameter and specify the name of a composite alarm, the operation returns information about the child alarms.\"\n    },\n    \"ParentsOfAlarmName\": {\n      \"type\": \"string\",\n      \"description\": \"If you use this\
  \ parameter and specify the name of a metric alarm, the operation returns information about the composite alarms that reference it.\"\n    },\n    \"ActionPrefix\": {\n      \"type\": \"string\",\n      \"description\": \"Use this parameter to filter the results to only those alarms that use a certain alarm action.\"\n    },\n    \"MaxRecords\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of alarm descriptions to retrieve.\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token returned by a previous call to indicate there is more data available.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-describe-alarms-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DescribeAlarmsInput
---
