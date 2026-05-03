---
description: Schema for a message processing log entry in SAP Cloud Integration
layout: schema
name: SAP Message Processing Log
properties_list:
- description: Unique GUID identifier for the message processing log entry
  name: MessageGuid
  type: string
- description: Correlation ID linking related messages across a process
  name: CorrelationId
  type: string
- description: Application-level message identifier
  name: ApplicationMessageId
  type: string
- description: Type classification of the application message
  name: ApplicationMessageType
  type: string
- description: ISO 8601 timestamp when message processing started
  name: LogStart
  type: string
- description: ISO 8601 timestamp when message processing ended
  name: LogEnd
  type: string
- description: Sending system, adapter, or channel identifier
  name: Sender
  type: string
- description: Receiving system, adapter, or channel identifier
  name: Receiver
  type: string
- description: Name of the integration flow that processed the message
  name: IntegrationFlowName
  type: string
- description: Current processing status of the message
  name: Status
  type: string
- description: Verbosity level of the log entry
  name: LogLevel
  type: string
provider_name: SAP Integration Suite
provider_slug: sap-integration-suite
schema_file: json-schema/sap-integration-suite-message-processing-log-schema.json
slug: sap-integration-suite-message-processing-log
source_filename: sap-integration-suite-message-processing-log-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sap-integration-suite/json-schema/sap-integration-suite-message-processing-log-schema.json\",\n  \"title\": \"SAP Message Processing Log\",\n  \"description\": \"Schema for a message processing log entry in SAP Cloud Integration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MessageGuid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique GUID identifier for the message processing log entry\"\n    },\n    \"CorrelationId\": {\n      \"type\": \"string\",\n      \"description\": \"Correlation ID linking related messages across a process\"\n    },\n    \"ApplicationMessageId\": {\n      \"type\": \"string\",\n      \"description\": \"Application-level message identifier\"\n    },\n    \"ApplicationMessageType\": {\n      \"type\": \"string\",\n      \"description\": \"Type classification of the application message\"\n    },\n    \"LogStart\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp when message processing started\",\n      \"format\": \"date-time\"\n    },\n    \"LogEnd\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp when message processing ended\",\n      \"format\": \"date-time\"\n    },\n    \"Sender\": {\n      \"type\": \"string\",\n      \"description\": \"Sending system, adapter, or channel identifier\"\n    },\n    \"Receiver\": {\n      \"type\": \"string\",\n      \"description\": \"Receiving system, adapter, or channel identifier\"\n    },\n    \"IntegrationFlowName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the integration flow that processed the message\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Current processing status of the message\",\n      \"enum\": [\"COMPLETED\", \"FAILED\", \"PROCESSING\", \"RETRY\", \"ESCALATED\", \"DISCARDED\", \"ABANDONED\"]\n    },\n    \"LogLevel\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Verbosity level of the log entry\",\n      \"enum\": [\"INFO\", \"DEBUG\", \"TRACE\", \"ERROR\"]\n    }\n  },\n  \"required\": [\"MessageGuid\", \"Status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/json-schema/sap-integration-suite-message-processing-log-schema.json
tags:
- API Management
- Cloud Integration
- Enterprise Integration
- Event Mesh
- iPaaS
- SAP
- SAP BTP
title: SAP Message Processing Log
---
