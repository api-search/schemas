---
description: <p>A JSON object containing the following fields:</p> <ul> <li> <p> <a>UpdateMaintenanceStartTimeInput$DayOfMonth</a> </p> </li> <li> <p> <a>UpdateMaintenanceStartTimeInput$DayOfWeek</a> </p> </li> <li> <p> <a>UpdateMaintenanceStartTimeInput$HourOfDay</a> </p> </li> <li> <p> <a>UpdateMaintenanceStartTimeInput$MinuteOfHour</a> </p> </li> </ul>
layout: schema
name: UpdateMaintenanceStartTimeInput
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
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-maintenance-start-time-input-schema.json
slug: amazon-storage-gateway-update-maintenance-start-time-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-maintenance-start-time-input-schema.json\",\n  \"title\": \"UpdateMaintenanceStartTimeInput\",\n  \"description\": \"<p>A JSON object containing the following fields:</p> <ul> <li> <p> <a>UpdateMaintenanceStartTimeInput$DayOfMonth</a> </p> </li> <li> <p> <a>UpdateMaintenanceStartTimeInput$DayOfWeek</a> </p> </li> <li> <p> <a>UpdateMaintenanceStartTimeInput$HourOfDay</a> </p> </li> <li> <p> <a>UpdateMaintenanceStartTimeInput$MinuteOfHour</a> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"HourOfDay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HourOfDay\"\n        },\n        {\n          \"description\": \"The hour component\
  \ of the maintenance start time represented as <i>hh</i>, where <i>hh</i> is the hour (00 to 23). The hour of the day is in the time zone of the gateway.\"\n        }\n      ]\n    },\n    \"MinuteOfHour\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinuteOfHour\"\n        },\n        {\n          \"description\": \"The minute component of the maintenance start time represented as <i>mm</i>, where <i>mm</i> is the minute (00 to 59). The minute of the hour is in the time zone of the gateway.\"\n        }\n      ]\n    },\n    \"DayOfWeek\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DayOfWeek\"\n        },\n        {\n          \"description\": \"The day of the week component of the maintenance start time week represented as an ordinal number from 0 to 6, where 0 represents Sunday and 6 Saturday.\"\n        }\n      ]\n    },\n    \"DayOfMonth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DayOfMonth\"\
  \n        },\n        {\n          \"description\": \"The day of the month component of the maintenance start time represented as an ordinal number from 1 to 28, where 1 represents the first day of the month and 28 represents the last day of the month.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"HourOfDay\",\n    \"MinuteOfHour\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-maintenance-start-time-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateMaintenanceStartTimeInput
---
