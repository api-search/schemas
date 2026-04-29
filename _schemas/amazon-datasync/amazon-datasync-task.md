---
description: Schema representing an AWS DataSync task resource. A task defines the source location, destination location, and the options to use for transferring data.
layout: schema
name: Amazon DataSync Task
properties_list:
- description: The Amazon Resource Name (ARN) of the task.
  name: TaskArn
  type: string
- description: The name of the task.
  name: Name
  type: string
- description: The status of the task.
  name: Status
  type: string
- description: The ARN of the source location for the task.
  name: SourceLocationArn
  type: string
- description: The ARN of the destination location for the task.
  name: DestinationLocationArn
  type: string
- description: The ARN of the most recent task execution.
  name: CurrentTaskExecutionArn
  type: string
- description: ''
  name: Options
  type: object
- description: ''
  name: Schedule
  type: object
- description: Errors that DataSync encountered during execution of the task.
  name: ErrorCode
  type: string
- description: Detailed description of an error that was encountered during the task execution.
  name: ErrorDetail
  type: string
- description: The time that the task was created.
  name: CreationTime
  type: string
- description: The tags associated with the task.
  name: Tags
  type: array
provider_name: Amazon DataSync
provider_slug: amazon-datasync
schema_file: json-schema/amazon-datasync-task-schema.json
slug: amazon-datasync-task
source_json: "{\n  \"$id\": \"https://schema.api.io/amazon-datasync/amazon-datasync-task-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Amazon DataSync Task\",\n  \"description\": \"Schema representing an AWS DataSync task resource. A task defines the source location, destination location, and the options to use for transferring data.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"TaskArn\",\n    \"SourceLocationArn\",\n    \"DestinationLocationArn\"\n  ],\n  \"properties\": {\n    \"TaskArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the task.\",\n      \"pattern\": \"^arn:aws:datasync:[a-z0-9-]+:[0-9]{12}:task/task-[a-f0-9]{17}$\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the task.\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the\
  \ task.\",\n      \"enum\": [\"AVAILABLE\", \"CREATING\", \"QUEUED\", \"RUNNING\", \"UNAVAILABLE\"]\n    },\n    \"SourceLocationArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the source location for the task.\"\n    },\n    \"DestinationLocationArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the destination location for the task.\"\n    },\n    \"CurrentTaskExecutionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the most recent task execution.\"\n    },\n    \"Options\": {\n      \"$ref\": \"#/$defs/Options\"\n    },\n    \"Schedule\": {\n      \"$ref\": \"#/$defs/TaskSchedule\"\n    },\n    \"ErrorCode\": {\n      \"type\": \"string\",\n      \"description\": \"Errors that DataSync encountered during execution of the task.\"\n    },\n    \"ErrorDetail\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of an error that was encountered during the task execution.\"\n    },\n\
  \    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time that the task was created.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"The tags associated with the task.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Options\": {\n      \"type\": \"object\",\n      \"description\": \"Represents the options that are available to control the behavior of a StartTaskExecution operation.\",\n      \"properties\": {\n        \"VerifyMode\": {\n          \"type\": \"string\",\n          \"enum\": [\"POINT_IN_TIME_CONSISTENT\", \"ONLY_FILES_TRANSFERRED\", \"NONE\"]\n        },\n        \"OverwriteMode\": {\n          \"type\": \"string\",\n          \"enum\": [\"ALWAYS\", \"NEVER\"]\n        },\n        \"Atime\": {\n          \"type\": \"string\",\n          \"enum\": [\"NONE\", \"BEST_EFFORT\"]\n        },\n        \"Mtime\": {\n          \"\
  type\": \"string\",\n          \"enum\": [\"NONE\", \"PRESERVE\"]\n        },\n        \"PreserveDeletedFiles\": {\n          \"type\": \"string\",\n          \"enum\": [\"PRESERVE\", \"REMOVE\"]\n        },\n        \"TransferMode\": {\n          \"type\": \"string\",\n          \"enum\": [\"CHANGED\", \"ALL\"]\n        },\n        \"LogLevel\": {\n          \"type\": \"string\",\n          \"enum\": [\"OFF\", \"BASIC\", \"TRANSFER\"]\n        }\n      }\n    },\n    \"TaskSchedule\": {\n      \"type\": \"object\",\n      \"required\": [\"ScheduleExpression\"],\n      \"properties\": {\n        \"ScheduleExpression\": {\n          \"type\": \"string\",\n          \"description\": \"A cron expression that specifies when DataSync initiates a scheduled transfer.\"\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"required\": [\"Key\"],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\"\
  : 256\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"maxLength\": 256\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datasync/refs/heads/main/json-schema/amazon-datasync-task-schema.json
tags:
- AWS
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
title: Amazon DataSync Task
---
