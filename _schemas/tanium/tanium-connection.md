---
description: Represents a data delivery connection in Tanium Connect. A connection links a data source (such as a saved question or event stream) to an external destination (such as a SIEM, file, or webhook) with configurable formatting, filtering, and scheduling.
layout: schema
name: Tanium Connect Connection
properties_list:
- description: Unique numeric identifier for the connection
  name: id
  type: integer
- description: Connection name
  name: name
  type: string
- description: Connection description
  name: description
  type: string
- description: Whether the connection is enabled and will run on schedule
  name: enabled
  type: boolean
- description: Data source configuration
  name: source
  type: object
- description: Destination configuration
  name: destination
  type: object
- description: Output format configuration
  name: format
  type: object
- description: Schedule configuration
  name: schedule
  type: object
- description: Status of the most recent execution
  name: lastRunStatus
  type: string
- description: Timestamp of the most recent execution
  name: lastRunTime
  type: string
- description: Connection creation timestamp
  name: createdAt
  type: string
- description: Connection last update timestamp
  name: updatedAt
  type: string
provider_name: Tanium
provider_slug: tanium
schema_file: json-schema/tanium-connection-schema.json
slug: tanium-connection
source_filename: tanium-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/tanium/blob/main/json-schema/tanium-connection-schema.json\",\n  \"title\": \"Tanium Connect Connection\",\n  \"description\": \"Represents a data delivery connection in Tanium Connect. A connection links a data source (such as a saved question or event stream) to an external destination (such as a SIEM, file, or webhook) with configurable formatting, filtering, and scheduling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the connection\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Connection name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Connection description\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the connection is enabled\
  \ and will run on schedule\"\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Data source identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Data source name\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Source type\",\n          \"enum\": [\"saved_question\", \"question_log\", \"system_status\", \"event\", \"discover\", \"integrity_monitor\", \"threat_response\"]\n        }\n      },\n      \"description\": \"Data source configuration\"\n    },\n    \"destination\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Destination identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Destination name\"\n        },\n        \"\
  type\": {\n          \"type\": \"string\",\n          \"description\": \"Destination type\",\n          \"enum\": [\"file\", \"syslog\", \"http\", \"email\", \"s3\", \"sql\"]\n        }\n      },\n      \"description\": \"Destination configuration\"\n    },\n    \"format\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Output format type\",\n          \"enum\": [\"csv\", \"json\", \"cef\", \"leef\", \"keyvalue\"]\n        },\n        \"options\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"delimiter\": {\n              \"type\": \"string\",\n              \"description\": \"Field delimiter for CSV format\"\n            },\n            \"headerRow\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether to include a header row\"\n            },\n            \"timestampFormat\": {\n              \"type\": \"string\",\n              \"\
  description\": \"Timestamp format string\"\n            }\n          }\n        }\n      },\n      \"description\": \"Output format configuration\"\n    },\n    \"schedule\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"intervalSeconds\": {\n          \"type\": \"integer\",\n          \"description\": \"Interval between runs in seconds\"\n        },\n        \"startTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Schedule start time\"\n        },\n        \"nextRunTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Next scheduled run time\"\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the schedule is active\"\n        }\n      },\n      \"description\": \"Schedule configuration\"\n    },\n    \"lastRunStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the most\
  \ recent execution\"\n    },\n    \"lastRunTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent execution\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Connection creation timestamp\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Connection last update timestamp\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/json-schema/tanium-connection-schema.json
tags:
- Compliance
- Endpoint Management
- Patch Management
- Security
- Threat Detection
- Unified Endpoint Management
title: Tanium Connect Connection
---
