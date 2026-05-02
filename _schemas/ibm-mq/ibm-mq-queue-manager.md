---
description: An IBM MQ queue manager is the primary component that hosts queues, topics, channels, and other MQ objects. It manages message storage, delivery, and routing for enterprise messaging.
layout: schema
name: IBM MQ Queue Manager
properties_list:
- description: Name of the queue manager
  name: name
  type: string
- description: Description of the queue manager
  name: description
  type: string
- description: Current operational state of the queue manager
  name: state
  type: string
- description: Platform the queue manager runs on
  name: platform
  type: string
- description: Command level indicating the MQ version capabilities
  name: commandLevel
  type: integer
- description: Maximum message length in bytes supported by the queue manager
  name: maximumMessageLength
  type: integer
- description: Name of the dead-letter queue for undeliverable messages
  name: deadLetterQueue
  type: string
- description: Name of the default transmission queue for remote messaging
  name: defaultTransmissionQueue
  type: string
- description: Coded character set identifier for the queue manager
  name: ccsid
  type: integer
- description: Trigger interval in milliseconds
  name: triggerInterval
  type: integer
- description: Number of current connections to the queue manager
  name: connectionCount
  type: integer
- description: State of the channel initiator
  name: channelInitiatorState
  type: string
- description: Timestamp when the queue manager was started
  name: started
  type: string
- description: ''
  name: listener
  type: object
provider_name: IBM MQ
provider_slug: ibm-mq
schema_file: json-schema/ibm-mq-queue-manager-schema.json
slug: ibm-mq-queue-manager
source_filename: ibm-mq-queue-manager-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.ibm.com/schemas/ibm-mq/queue-manager.json\",\n  \"title\": \"IBM MQ Queue Manager\",\n  \"description\": \"An IBM MQ queue manager is the primary component that hosts queues, topics, channels, and other MQ objects. It manages message storage, delivery, and routing for enterprise messaging.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the queue manager\",\n      \"minLength\": 1,\n      \"maxLength\": 48,\n      \"pattern\": \"^[A-Za-z0-9._/%]+$\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the queue manager\",\n      \"maxLength\": 64\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"running\", \"ended\"],\n      \"description\": \"Current operational state of the queue manager\"\n    },\n\
  \    \"platform\": {\n      \"type\": \"string\",\n      \"enum\": [\"unix\", \"windows\", \"appliance\", \"zos\"],\n      \"description\": \"Platform the queue manager runs on\"\n    },\n    \"commandLevel\": {\n      \"type\": \"integer\",\n      \"description\": \"Command level indicating the MQ version capabilities\"\n    },\n    \"maximumMessageLength\": {\n      \"type\": \"integer\",\n      \"minimum\": 32,\n      \"maximum\": 104857600,\n      \"description\": \"Maximum message length in bytes supported by the queue manager\"\n    },\n    \"deadLetterQueue\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the dead-letter queue for undeliverable messages\",\n      \"maxLength\": 48\n    },\n    \"defaultTransmissionQueue\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the default transmission queue for remote messaging\",\n      \"maxLength\": 48\n    },\n    \"ccsid\": {\n      \"type\": \"integer\",\n      \"description\": \"Coded character\
  \ set identifier for the queue manager\"\n    },\n    \"triggerInterval\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Trigger interval in milliseconds\"\n    },\n    \"connectionCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of current connections to the queue manager\"\n    },\n    \"channelInitiatorState\": {\n      \"type\": \"string\",\n      \"enum\": [\"running\", \"stopped\"],\n      \"description\": \"State of the channel initiator\"\n    },\n    \"started\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the queue manager was started\"\n    },\n    \"listener\": {\n      \"$ref\": \"#/$defs/Listener\"\n    }\n  },\n  \"$defs\": {\n    \"Listener\": {\n      \"type\": \"object\",\n      \"description\": \"Queue manager listener configuration\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n         \
  \ \"description\": \"Listener name\"\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 65535,\n          \"description\": \"TCP/IP port number\"\n        },\n        \"transportType\": {\n          \"type\": \"string\",\n          \"enum\": [\"tcp\", \"lu62\", \"netbios\", \"spx\"],\n          \"description\": \"Transport type for the listener\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\"running\", \"stopped\"],\n          \"description\": \"Current state of the listener\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/json-schema/ibm-mq-queue-manager-schema.json
tags:
- Async
- Enterprise
- Integration
- Messaging
- Middleware
- Queue
title: IBM MQ Queue Manager
---
