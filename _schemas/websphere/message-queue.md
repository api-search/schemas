---
description: Represents an IBM MQ message queue including its configuration, runtime status, depth, and messaging properties for point-to-point and publish-subscribe messaging patterns.
layout: schema
name: IBM MQ Message Queue
properties_list:
- description: The unique name of the queue within the queue manager.
  name: name
  type: string
- description: Human-readable display name for the queue.
  name: displayName
  type: string
- description: Description of the queue purpose.
  name: description
  type: string
- description: Queue type.
  name: type
  type: string
- description: Name of the queue manager that owns this queue.
  name: queueManager
  type: string
- description: Maximum number of messages that can be held on the queue.
  name: maxDepth
  type: integer
- description: Maximum length of a message in bytes.
  name: maxMessageLength
  type: integer
- description: Current number of messages on the queue.
  name: currentDepth
  type: integer
- description: Message persistence configuration.
  name: persistence
  type: object
- description: Whether put operations are inhibited on this queue.
  name: inhibitPut
  type: boolean
- description: Whether get operations are inhibited on this queue.
  name: inhibitGet
  type: boolean
- description: Triggering configuration for the queue.
  name: triggerControl
  type: object
- description: Cluster queue properties (for cluster queues).
  name: cluster
  type: object
- description: Name of the dead letter queue for undeliverable messages.
  name: deadLetterQueue
  type: string
- description: Number of times a message can be backed out before being moved to the backout queue.
  name: backoutThreshold
  type: integer
- description: Name of the backout requeue queue.
  name: backoutQueue
  type: string
- description: Whether the queue can be opened for input by multiple applications.
  name: shareability
  type: string
- description: Default input open option.
  name: defaultInputOpenOption
  type: string
- description: Message priority settings.
  name: messagePriority
  type: object
- description: Runtime status information.
  name: status
  type: object
- description: Alias queue properties (for alias queues).
  name: alias
  type: object
- description: Remote queue properties (for remote queues).
  name: remote
  type: object
- description: Date and time the queue was created.
  name: createdDate
  type: string
- description: Date and time the queue was last modified.
  name: lastModified
  type: string
- description: Additional metadata associated with the queue.
  name: metadata
  type: object
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/message-queue.json
slug: message-queue
source_filename: message-queue.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"message-queue.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IBM MQ Message Queue\",\n  \"description\": \"Represents an IBM MQ message queue including its configuration, runtime status, depth, and messaging properties for point-to-point and publish-subscribe messaging patterns.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 48,\n      \"description\": \"The unique name of the queue within the queue manager.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name for the queue.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"maxLength\": 64,\n      \"description\": \"Description of the queue purpose.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"local\", \"alias\", \"remote\", \"model\", \"cluster\"],\n      \"description\": \"Queue type.\"\
  \n    },\n    \"queueManager\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the queue manager that owns this queue.\"\n    },\n    \"maxDepth\": {\n      \"type\": \"integer\",\n      \"default\": 5000,\n      \"minimum\": 0,\n      \"maximum\": 999999999,\n      \"description\": \"Maximum number of messages that can be held on the queue.\"\n    },\n    \"maxMessageLength\": {\n      \"type\": \"integer\",\n      \"default\": 4194304,\n      \"minimum\": 0,\n      \"maximum\": 104857600,\n      \"description\": \"Maximum length of a message in bytes.\"\n    },\n    \"currentDepth\": {\n      \"type\": \"integer\",\n      \"description\": \"Current number of messages on the queue.\",\n      \"readOnly\": true\n    },\n    \"persistence\": {\n      \"type\": \"object\",\n      \"description\": \"Message persistence configuration.\",\n      \"properties\": {\n        \"default\": {\n          \"type\": \"string\",\n          \"enum\": [\"persistent\", \"nonPersistent\"\
  ],\n          \"default\": \"persistent\",\n          \"description\": \"Default persistence for messages put on this queue.\"\n        }\n      }\n    },\n    \"inhibitPut\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether put operations are inhibited on this queue.\"\n    },\n    \"inhibitGet\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether get operations are inhibited on this queue.\"\n    },\n    \"triggerControl\": {\n      \"type\": \"object\",\n      \"description\": \"Triggering configuration for the queue.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether triggering is enabled.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"NONE\", \"FIRST\", \"EVERY\", \"DEPTH\"],\n          \"description\": \"Trigger type.\"\n        },\n        \"depth\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Trigger depth threshold.\"\n        },\n        \"messageType\": {\n          \"type\": \"integer\",\n          \"description\": \"Message type for triggering.\"\n        },\n        \"processName\": {\n          \"type\": \"string\",\n          \"description\": \"Process to initiate when triggered.\"\n        },\n        \"initializationQueue\": {\n          \"type\": \"string\",\n          \"description\": \"Initiation queue name.\"\n        }\n      }\n    },\n    \"cluster\": {\n      \"type\": \"object\",\n      \"description\": \"Cluster queue properties (for cluster queues).\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Cluster name.\"\n        },\n        \"workloadRank\": {\n          \"type\": \"integer\",\n          \"description\": \"Cluster workload rank.\"\n        },\n        \"workloadPriority\": {\n          \"type\": \"integer\",\n    \
  \      \"description\": \"Cluster workload priority.\"\n        },\n        \"workloadUseQueue\": {\n          \"type\": \"string\",\n          \"enum\": [\"local\", \"any\"],\n          \"description\": \"Cluster workload queue usage.\"\n        }\n      }\n    },\n    \"deadLetterQueue\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the dead letter queue for undeliverable messages.\"\n    },\n    \"backoutThreshold\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times a message can be backed out before being moved to the backout queue.\"\n    },\n    \"backoutQueue\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the backout requeue queue.\"\n    },\n    \"shareability\": {\n      \"type\": \"string\",\n      \"enum\": [\"shareable\", \"notShareable\"],\n      \"default\": \"shareable\",\n      \"description\": \"Whether the queue can be opened for input by multiple applications.\"\n    },\n    \"defaultInputOpenOption\":\
  \ {\n      \"type\": \"string\",\n      \"enum\": [\"shared\", \"exclusive\"],\n      \"default\": \"shared\",\n      \"description\": \"Default input open option.\"\n    },\n    \"messagePriority\": {\n      \"type\": \"object\",\n      \"description\": \"Message priority settings.\",\n      \"properties\": {\n        \"default\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 9,\n          \"description\": \"Default message priority.\"\n        },\n        \"deliverySequence\": {\n          \"type\": \"string\",\n          \"enum\": [\"priority\", \"fifo\"],\n          \"default\": \"priority\",\n          \"description\": \"Message delivery sequence.\"\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"description\": \"Runtime status information.\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"currentDepth\": {\n          \"type\": \"integer\",\n          \"description\": \"Current number of\
  \ messages.\"\n        },\n        \"openInputCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of applications with the queue open for input.\"\n        },\n        \"openOutputCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of applications with the queue open for output.\"\n        },\n        \"lastGetDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Date and time of the last successful get operation.\"\n        },\n        \"lastPutDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Date and time of the last successful put operation.\"\n        },\n        \"uncommittedMessages\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of uncommitted messages.\"\n        },\n        \"oldestMessageAge\": {\n          \"type\": \"integer\",\n          \"description\": \"Age of\
  \ the oldest message in seconds.\"\n        }\n      }\n    },\n    \"alias\": {\n      \"type\": \"object\",\n      \"description\": \"Alias queue properties (for alias queues).\",\n      \"properties\": {\n        \"targetQueue\": {\n          \"type\": \"string\",\n          \"description\": \"Target queue name that this alias resolves to.\"\n        },\n        \"targetType\": {\n          \"type\": \"string\",\n          \"enum\": [\"queue\", \"topic\"],\n          \"description\": \"Target object type.\"\n        }\n      }\n    },\n    \"remote\": {\n      \"type\": \"object\",\n      \"description\": \"Remote queue properties (for remote queues).\",\n      \"properties\": {\n        \"remoteQueueName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the queue on the remote queue manager.\"\n        },\n        \"remoteQueueManager\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the remote queue manager.\"\n        },\n     \
  \   \"transmissionQueue\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the transmission queue.\"\n        }\n      }\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the queue was created.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the queue was last modified.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Additional metadata associated with the queue.\"\n    }\n  },\n  \"required\": [\"name\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/message-queue.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: IBM MQ Message Queue
---
