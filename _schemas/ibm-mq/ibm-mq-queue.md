---
description: An IBM MQ queue is a named object that stores messages for asynchronous consumption. Queues can be local, alias, remote, model, or cluster types, each serving different messaging patterns.
layout: schema
name: IBM MQ Queue
properties_list:
- description: Name of the queue
  name: name
  type: string
- description: Type of the queue
  name: type
  type: string
- description: Description of the queue
  name: description
  type: string
- description: Maximum number of messages that can be stored on the queue
  name: maximumDepth
  type: integer
- description: Maximum message length in bytes for messages on this queue
  name: maximumMessageLength
  type: integer
- description: Whether put operations are inhibited on this queue
  name: inhibitPut
  type: boolean
- description: Whether get operations are inhibited on this queue
  name: inhibitGet
  type: boolean
- description: Default persistence for messages put on this queue
  name: defaultPersistence
  type: string
- description: Default priority for messages put on this queue
  name: defaultPriority
  type: integer
- description: Number of times a message can be backed out before being moved
  name: backoutThreshold
  type: integer
- description: Queue to which messages are moved after exceeding the backout threshold
  name: backoutRequeueQueue
  type: string
- description: Whether this queue is used as a transmission queue for remote messaging
  name: isTransmissionQueue
  type: boolean
- description: Whether triggering is enabled for this queue
  name: triggerControl
  type: string
- description: Type of triggering configured for this queue
  name: triggerType
  type: string
- description: Whether the queue can be opened by multiple applications simultaneously
  name: shareability
  type: string
- description: Current number of messages on the queue
  name: currentDepth
  type: integer
- description: Number of handles currently open for input (get)
  name: openInputCount
  type: integer
- description: Number of handles currently open for output (put)
  name: openOutputCount
  type: integer
- description: Timestamp of the last message put on the queue
  name: lastPut
  type: string
- description: Timestamp of the last message retrieved from the queue
  name: lastGet
  type: string
- description: ''
  name: alias
  type: object
- description: ''
  name: remote
  type: object
- description: ''
  name: cluster
  type: object
provider_name: IBM MQ
provider_slug: ibm-mq
schema_file: json-schema/ibm-mq-queue-schema.json
slug: ibm-mq-queue
source_filename: ibm-mq-queue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.ibm.com/schemas/ibm-mq/queue.json\",\n  \"title\": \"IBM MQ Queue\",\n  \"description\": \"An IBM MQ queue is a named object that stores messages for asynchronous consumption. Queues can be local, alias, remote, model, or cluster types, each serving different messaging patterns.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"type\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the queue\",\n      \"minLength\": 1,\n      \"maxLength\": 48,\n      \"pattern\": \"^[A-Za-z0-9._/%]+$\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"local\", \"alias\", \"remote\", \"model\", \"cluster\"],\n      \"description\": \"Type of the queue\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the queue\",\n      \"maxLength\": 64\n    },\n    \"maximumDepth\"\
  : {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 999999999,\n      \"description\": \"Maximum number of messages that can be stored on the queue\"\n    },\n    \"maximumMessageLength\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 104857600,\n      \"description\": \"Maximum message length in bytes for messages on this queue\"\n    },\n    \"inhibitPut\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether put operations are inhibited on this queue\"\n    },\n    \"inhibitGet\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether get operations are inhibited on this queue\"\n    },\n    \"defaultPersistence\": {\n      \"type\": \"string\",\n      \"enum\": [\"persistent\", \"notPersistent\"],\n      \"description\": \"Default persistence for messages put on this queue\"\n    },\n    \"defaultPriority\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 9,\n      \"description\"\
  : \"Default priority for messages put on this queue\"\n    },\n    \"backoutThreshold\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of times a message can be backed out before being moved\"\n    },\n    \"backoutRequeueQueue\": {\n      \"type\": \"string\",\n      \"description\": \"Queue to which messages are moved after exceeding the backout threshold\",\n      \"maxLength\": 48\n    },\n    \"isTransmissionQueue\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this queue is used as a transmission queue for remote messaging\"\n    },\n    \"triggerControl\": {\n      \"type\": \"string\",\n      \"enum\": [\"on\", \"off\"],\n      \"description\": \"Whether triggering is enabled for this queue\"\n    },\n    \"triggerType\": {\n      \"type\": \"string\",\n      \"enum\": [\"none\", \"first\", \"every\", \"depth\"],\n      \"description\": \"Type of triggering configured for this queue\"\n    },\n    \"shareability\":\
  \ {\n      \"type\": \"string\",\n      \"enum\": [\"shareable\", \"notShareable\"],\n      \"description\": \"Whether the queue can be opened by multiple applications simultaneously\"\n    },\n    \"currentDepth\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Current number of messages on the queue\"\n    },\n    \"openInputCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of handles currently open for input (get)\"\n    },\n    \"openOutputCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of handles currently open for output (put)\"\n    },\n    \"lastPut\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last message put on the queue\"\n    },\n    \"lastGet\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last message retrieved from the\
  \ queue\"\n    },\n    \"alias\": {\n      \"$ref\": \"#/$defs/AliasProperties\"\n    },\n    \"remote\": {\n      \"$ref\": \"#/$defs/RemoteProperties\"\n    },\n    \"cluster\": {\n      \"$ref\": \"#/$defs/ClusterProperties\"\n    }\n  },\n  \"$defs\": {\n    \"AliasProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Properties specific to alias queues\",\n      \"properties\": {\n        \"baseQueueName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the base queue or topic that this alias resolves to\"\n        },\n        \"baseType\": {\n          \"type\": \"string\",\n          \"enum\": [\"queue\", \"topic\"],\n          \"description\": \"Whether the alias resolves to a queue or topic\"\n        }\n      }\n    },\n    \"RemoteProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Properties specific to remote queue definitions\",\n      \"properties\": {\n        \"remoteQueueName\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Name of the queue on the remote queue manager\"\n        },\n        \"remoteQueueManager\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the remote queue manager\"\n        },\n        \"transmissionQueue\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the transmission queue to use\"\n        }\n      }\n    },\n    \"ClusterProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Properties specific to cluster queues\",\n      \"properties\": {\n        \"clusterName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the cluster this queue belongs to\"\n        },\n        \"clusterNamelist\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the namelist of clusters this queue belongs to\"\n        },\n        \"defaultBind\": {\n          \"type\": \"string\",\n          \"enum\": [\"onOpen\", \"notFixed\", \"onGroup\"],\n          \"\
  description\": \"Default binding for cluster queue\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/json-schema/ibm-mq-queue-schema.json
tags:
- Async
- Enterprise
- Integration
- Messaging
- Middleware
- Queue
title: IBM MQ Queue
---
