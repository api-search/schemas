---
description: <p>A JSON object containing the following fields:</p> <ul> <li> <p> <a>DescribeMaintenanceStartTimeOutput$DayOfMonth</a> </p> </li> <li> <p> <a>DescribeMaintenanceStartTimeOutput$DayOfWeek</a> </p> </li> <li> <p> <a>DescribeMaintenanceStartTimeOutput$HourOfDay</a> </p> </li> <li> <p> <a>DescribeMaintenanceStartTimeOutput$MinuteOfHour</a> </p> </li> <li> <p> <a>DescribeMaintenanceStartTimeOutput$Timezone</a> </p> </li> </ul>
layout: schema
name: DescribeMaintenanceStartTimeOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: HourOfDay
  type: object
- description: ''
  name: MinuteOfHour
  type: object
- description: ''
  name: DayOfWeek
  type: object
- description: ''
  name: DayOfMonth
  type: object
- description: ''
  name: Timezone
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-maintenance-start-time-output-schema.json
slug: amazon-storage-gateway-describe-maintenance-start-time-output
source_filename: amazon-storage-gateway-describe-maintenance-start-time-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-maintenance-start-time-output-schema.json\",\n  \"title\": \"DescribeMaintenanceStartTimeOutput\",\n  \"description\": \"<p>A JSON object containing the following fields:</p> <ul> <li> <p> <a>DescribeMaintenanceStartTimeOutput$DayOfMonth</a> </p> </li> <li> <p> <a>DescribeMaintenanceStartTimeOutput$DayOfWeek</a> </p> </li> <li> <p> <a>DescribeMaintenanceStartTimeOutput$HourOfDay</a> </p> </li> <li> <p> <a>DescribeMaintenanceStartTimeOutput$MinuteOfHour</a> </p> </li> <li> <p> <a>DescribeMaintenanceStartTimeOutput$Timezone</a> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"HourOfDay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HourOfDay\"\
  \n        },\n        {\n          \"description\": \"The hour component of the maintenance start time represented as <i>hh</i>, where <i>hh</i> is the hour (0 to 23). The hour of the day is in the time zone of the gateway.\"\n        }\n      ]\n    },\n    \"MinuteOfHour\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinuteOfHour\"\n        },\n        {\n          \"description\": \"The minute component of the maintenance start time represented as <i>mm</i>, where <i>mm</i> is the minute (0 to 59). The minute of the hour is in the time zone of the gateway.\"\n        }\n      ]\n    },\n    \"DayOfWeek\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DayOfWeek\"\n        },\n        {\n          \"description\": \"An ordinal number between 0 and 6 that represents the day of the week, where 0 represents Sunday and 6 represents Saturday. The day of week is in the time zone of the gateway.\"\n        }\n      ]\n    },\n \
  \   \"DayOfMonth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DayOfMonth\"\n        },\n        {\n          \"description\": \"The day of the month component of the maintenance start time represented as an ordinal number from 1 to 28, where 1 represents the first day of the month and 28 represents the last day of the month.\"\n        }\n      ]\n    },\n    \"Timezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayTimezone\"\n        },\n        {\n          \"description\": \"A value that indicates the time zone that is set for the gateway. The start time and day of week specified should be in the time zone of the gateway.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-maintenance-start-time-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeMaintenanceStartTimeOutput
---
