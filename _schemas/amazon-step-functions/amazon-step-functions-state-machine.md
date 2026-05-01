---
description: Represents an Amazon Step Functions state machine with its associated configuration, definition, and metadata.
layout: schema
name: Amazon Step Functions State Machine
properties_list:
- description: The ARN that identifies the state machine
  name: stateMachineArn
  type: string
- description: The name of the state machine
  name: name
  type: string
- description: The current status of the state machine
  name: status
  type: string
- description: The Amazon States Language definition of the state machine as a JSON string
  name: definition
  type: string
- description: The ARN of the IAM role used by the state machine for executions
  name: roleArn
  type: string
- description: The type of the state machine (STANDARD or EXPRESS)
  name: type
  type: string
- description: The date the state machine was created
  name: creationDate
  type: string
- description: ''
  name: loggingConfiguration
  type: object
- description: ''
  name: tracingConfiguration
  type: object
- description: A user-defined or auto-generated string that identifies a Map state
  name: label
  type: string
- description: The revision identifier for the state machine
  name: revisionId
  type: string
- description: A user-defined description of the state machine
  name: description
  type: string
- description: Tags attached to the state machine
  name: tags
  type: array
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-state-machine-schema.json
slug: amazon-step-functions-state-machine
source_filename: amazon-step-functions-state-machine-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/step-functions/state-machine.json\",\n  \"title\": \"Amazon Step Functions State Machine\",\n  \"description\": \"Represents an Amazon Step Functions state machine with its associated configuration, definition, and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"stateMachineArn\", \"name\", \"definition\", \"roleArn\", \"type\", \"creationDate\"],\n  \"properties\": {\n    \"stateMachineArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN that identifies the state machine\",\n      \"pattern\": \"^arn:aws:states:[a-z0-9-]+:\\\\d{12}:stateMachine:.+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the state machine\",\n      \"minLength\": 1,\n      \"maxLength\": 80\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the state\
  \ machine\",\n      \"enum\": [\"ACTIVE\", \"DELETING\"]\n    },\n    \"definition\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon States Language definition of the state machine as a JSON string\"\n    },\n    \"roleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the IAM role used by the state machine for executions\",\n      \"pattern\": \"^arn:aws:iam::\\\\d{12}:role/.+$\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the state machine (STANDARD or EXPRESS)\",\n      \"enum\": [\"STANDARD\", \"EXPRESS\"]\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date the state machine was created\"\n    },\n    \"loggingConfiguration\": {\n      \"$ref\": \"#/$defs/LoggingConfiguration\"\n    },\n    \"tracingConfiguration\": {\n      \"$ref\": \"#/$defs/TracingConfiguration\"\n    },\n    \"label\": {\n      \"type\": \"\
  string\",\n      \"description\": \"A user-defined or auto-generated string that identifies a Map state\"\n    },\n    \"revisionId\": {\n      \"type\": \"string\",\n      \"description\": \"The revision identifier for the state machine\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A user-defined description of the state machine\",\n      \"maxLength\": 256\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags attached to the state machine\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"LoggingConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Logging configuration for the state machine\",\n      \"properties\": {\n        \"level\": {\n          \"type\": \"string\",\n          \"description\": \"Defines which category of execution history events are logged\",\n          \"enum\": [\"ALL\", \"ERROR\", \"FATAL\", \"OFF\"]\n        },\n\
  \        \"includeExecutionData\": {\n          \"type\": \"boolean\",\n          \"description\": \"Determines whether execution data is included in log messages\"\n        },\n        \"destinations\": {\n          \"type\": \"array\",\n          \"description\": \"Array of objects that describe where logs are sent\",\n          \"items\": {\n            \"$ref\": \"#/$defs/LogDestination\"\n          }\n        }\n      }\n    },\n    \"LogDestination\": {\n      \"type\": \"object\",\n      \"description\": \"A log destination configuration\",\n      \"properties\": {\n        \"cloudWatchLogsLogGroup\": {\n          \"type\": \"object\",\n          \"description\": \"CloudWatch Logs log group configuration\",\n          \"properties\": {\n            \"logGroupArn\": {\n              \"type\": \"string\",\n              \"description\": \"The ARN of the CloudWatch Logs log group\"\n            }\n          }\n        }\n      }\n    },\n    \"TracingConfiguration\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"X-Ray tracing configuration for the state machine\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"When set to true, X-Ray tracing is enabled\"\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a resource tag\",\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the tag\",\n          \"maxLength\": 128\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value of the tag\",\n          \"maxLength\": 256\n        }\n      },\n      \"required\": [\"key\"]\n    },\n    \"StateMachineDefinition\": {\n      \"type\": \"object\",\n      \"description\": \"The Amazon States Language definition structure\",\n      \"required\": [\"StartAt\", \"States\"],\n      \"properties\": {\n        \"Comment\": {\n          \"\
  type\": \"string\",\n          \"description\": \"A human-readable description of the state machine\"\n        },\n        \"StartAt\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the state where execution starts\"\n        },\n        \"States\": {\n          \"type\": \"object\",\n          \"description\": \"An object containing a set of states\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/State\"\n          }\n        },\n        \"TimeoutSeconds\": {\n          \"type\": \"integer\",\n          \"description\": \"The maximum number of seconds an execution can run\",\n          \"minimum\": 0\n        },\n        \"Version\": {\n          \"type\": \"string\",\n          \"description\": \"The version of the Amazon States Language\"\n        }\n      }\n    },\n    \"State\": {\n      \"type\": \"object\",\n      \"description\": \"A single state in the state machine\",\n      \"required\": [\"Type\"],\n      \"properties\"\
  : {\n        \"Type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of the state\",\n          \"enum\": [\"Task\", \"Pass\", \"Choice\", \"Wait\", \"Succeed\", \"Fail\", \"Parallel\", \"Map\"]\n        },\n        \"Comment\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable description of the state\"\n        },\n        \"InputPath\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A path that selects a portion of the state input\"\n        },\n        \"OutputPath\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A path that selects a portion of the state output\"\n        },\n        \"Next\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the next state to transition to\"\n        },\n        \"End\": {\n          \"type\": \"boolean\",\n          \"description\": \"Designates this state as a terminal state\"\n        },\n        \"\
  Resource\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the resource to invoke (for Task states)\"\n        },\n        \"Parameters\": {\n          \"type\": \"object\",\n          \"description\": \"Key-value pairs passed as input to the resource\"\n        },\n        \"ResultPath\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A path that determines what is sent as input to the next state\"\n        },\n        \"ResultSelector\": {\n          \"type\": \"object\",\n          \"description\": \"Key-value pairs to manipulate the result before ResultPath\"\n        },\n        \"Retry\": {\n          \"type\": \"array\",\n          \"description\": \"Retry policies for the state\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Retrier\"\n          }\n        },\n        \"Catch\": {\n          \"type\": \"array\",\n          \"description\": \"Catch clauses for error handling\",\n          \"items\": {\n     \
  \       \"$ref\": \"#/$defs/Catcher\"\n          }\n        },\n        \"Choices\": {\n          \"type\": \"array\",\n          \"description\": \"Array of choice rules (for Choice states)\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        },\n        \"Default\": {\n          \"type\": \"string\",\n          \"description\": \"The default state for a Choice state\"\n        },\n        \"Seconds\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of seconds to wait (for Wait states)\"\n        },\n        \"Timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"An absolute time to wait until (for Wait states)\"\n        },\n        \"Branches\": {\n          \"type\": \"array\",\n          \"description\": \"Array of parallel branches (for Parallel states)\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        },\n        \"Iterator\":\
  \ {\n          \"type\": \"object\",\n          \"description\": \"The state machine to process each array element (for Map states)\"\n        },\n        \"ItemsPath\": {\n          \"type\": \"string\",\n          \"description\": \"Reference path identifying the array to iterate over (for Map states)\"\n        },\n        \"MaxConcurrency\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum concurrent iterations (for Map states)\",\n          \"minimum\": 0\n        },\n        \"Error\": {\n          \"type\": \"string\",\n          \"description\": \"The error name for a Fail state\"\n        },\n        \"Cause\": {\n          \"type\": \"string\",\n          \"description\": \"A description for a Fail state\"\n        },\n        \"TimeoutSeconds\": {\n          \"type\": \"integer\",\n          \"description\": \"The maximum time in seconds a Task state can run\"\n        },\n        \"HeartbeatSeconds\": {\n          \"type\": \"integer\",\n          \"\
  description\": \"The time between heartbeats for a Task state\"\n        }\n      }\n    },\n    \"Retrier\": {\n      \"type\": \"object\",\n      \"description\": \"A retry policy\",\n      \"required\": [\"ErrorEquals\"],\n      \"properties\": {\n        \"ErrorEquals\": {\n          \"type\": \"array\",\n          \"description\": \"The error names to match\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"IntervalSeconds\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of seconds before the first retry attempt\",\n          \"minimum\": 1\n        },\n        \"MaxAttempts\": {\n          \"type\": \"integer\",\n          \"description\": \"The maximum number of retry attempts\",\n          \"minimum\": 0\n        },\n        \"BackoffRate\": {\n          \"type\": \"number\",\n          \"description\": \"The multiplier by which the retry interval increases\",\n          \"minimum\": 1.0\n        }\n \
  \     }\n    },\n    \"Catcher\": {\n      \"type\": \"object\",\n      \"description\": \"A catch clause for error handling\",\n      \"required\": [\"ErrorEquals\", \"Next\"],\n      \"properties\": {\n        \"ErrorEquals\": {\n          \"type\": \"array\",\n          \"description\": \"The error names to match\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"Next\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the state to transition to\"\n        },\n        \"ResultPath\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A path that determines what is sent as input to the Next state\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-state-machine-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: Amazon Step Functions State Machine
---
