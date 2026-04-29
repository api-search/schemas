---
description: A Boltic Pipe is a data synchronization pipeline that connects a data source to a destination with configurable scheduling and field mappings.
layout: schema
name: Boltic Pipe
properties_list:
- description: Unique identifier for the pipe
  name: id
  type: string
- description: Human-readable name for the pipe
  name: name
  type: string
- description: Description of the data sync pipeline
  name: description
  type: string
- description: Current status of the pipe
  name: status
  type: string
- description: ''
  name: source
  type: object
- description: ''
  name: destination
  type: object
- description: ''
  name: schedule
  type: object
- description: Timestamp of the last successful sync
  name: lastSyncAt
  type: string
- description: Total rows synced since creation
  name: rowsSynced
  type: integer
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Boltic
provider_slug: boltic
schema_file: json-schema/boltic-pipe.json
slug: boltic-pipe
source_filename: boltic-pipe.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/json-schema/boltic-pipe.json\",\n  \"title\": \"Boltic Pipe\",\n  \"description\": \"A Boltic Pipe is a data synchronization pipeline that connects a data source to a destination with configurable scheduling and field mappings.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"source\", \"destination\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the pipe\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the pipe\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the data sync pipeline\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"paused\", \"error\"],\n      \"description\": \"Current status\
  \ of the pipe\"\n    },\n    \"source\": {\n      \"$ref\": \"#/$defs/sourceConfig\"\n    },\n    \"destination\": {\n      \"$ref\": \"#/$defs/destinationConfig\"\n    },\n    \"schedule\": {\n      \"$ref\": \"#/$defs/schedule\"\n    },\n    \"lastSyncAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last successful sync\"\n    },\n    \"rowsSynced\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Total rows synced since creation\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$defs\": {\n    \"sourceConfig\": {\n      \"type\": \"object\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Source type (e.g., mongodb, mysql, postgresql, rest-api)\"\
  \n        },\n        \"connectionConfig\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Connection parameters specific to the source type\"\n        },\n        \"rootPath\": {\n          \"type\": \"string\",\n          \"description\": \"Root path for REST API data extraction\"\n        },\n        \"authType\": {\n          \"type\": \"string\",\n          \"enum\": [\"none\", \"basic\", \"bearer\", \"oauth2\", \"api-key\"]\n        },\n        \"authConfig\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"destinationConfig\": {\n      \"type\": \"object\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Destination type identifier\"\n        },\n        \"connectionConfig\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        },\n\
  \        \"mappings\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"sourceField\": { \"type\": \"string\" },\n              \"destinationField\": { \"type\": \"string\" },\n              \"transformation\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    },\n    \"schedule\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"frequency\": {\n          \"type\": \"string\",\n          \"enum\": [\"minutely\", \"hourly\", \"daily\", \"weekly\", \"monthly\", \"custom\"]\n        },\n        \"interval\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Interval value for the frequency\"\n        },\n        \"cronExpression\": {\n          \"type\": \"string\",\n          \"description\": \"Cron expression for custom schedules\"\n        },\n        \"timezone\": {\n          \"type\": \"string\"\n       \
  \ }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/boltic/refs/heads/main/json-schema/boltic-pipe.json
tags:
- Automation
- DataSync
- Gateways
- NoCode
- Streaming
- Workflows
title: Boltic Pipe
---
