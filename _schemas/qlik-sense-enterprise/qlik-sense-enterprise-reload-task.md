---
description: A reload task defines a scheduled or manually triggered operation to reload data in a Qlik Sense application from its connected data sources. Tasks track execution history, status, and can be configured with retry policies and triggers.
layout: schema
name: Qlik Sense Reload Task
properties_list:
- description: Unique identifier (GUID) assigned by the repository
  name: id
  type: string
- description: ISO 8601 timestamp when the task was created
  name: createdDate
  type: string
- description: ISO 8601 timestamp when the task was last modified
  name: modifiedDate
  type: string
- description: Username of the user who last modified the task
  name: modifiedByUserName
  type: string
- description: Display name of the reload task
  name: name
  type: string
- description: Task type identifier (0=ReloadTask)
  name: taskType
  type: integer
- description: Whether the task is enabled for execution
  name: enabled
  type: boolean
- description: Maximum execution time in minutes before the task is terminated
  name: taskSessionTimeout
  type: integer
- description: Maximum number of automatic retry attempts on failure
  name: maxRetries
  type: integer
- description: The application this reload task is associated with
  name: app
  type: object
- description: Whether the task requires manual triggering rather than scheduled execution
  name: isManuallyTriggered
  type: boolean
- description: Operational information including last execution result and next execution time
  name: operational
  type: object
- description: Tags applied to the task
  name: tags
  type: array
- description: Custom property values assigned to the task
  name: customProperties
  type: array
- description: List of privileges the current user has on this task
  name: privileges
  type: array
- description: Schema path identifying the entity type in the QRS
  name: schemaPath
  type: string
provider_name: Qlik Sense Enterprise
provider_slug: qlik-sense-enterprise
schema_file: json-schema/qlik-sense-enterprise-reload-task-schema.json
slug: qlik-sense-enterprise-reload-task
source_filename: qlik-sense-enterprise-reload-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api.dev/qlik-sense-enterprise/reload-task.json\",\n  \"title\": \"Qlik Sense Reload Task\",\n  \"description\": \"A reload task defines a scheduled or manually triggered operation to reload data in a Qlik Sense application from its connected data sources. Tasks track execution history, status, and can be configured with retry policies and triggers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier (GUID) assigned by the repository\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the task was created\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the task was last modified\"\
  \n    },\n    \"modifiedByUserName\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the user who last modified the task\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the reload task\",\n      \"minLength\": 1\n    },\n    \"taskType\": {\n      \"type\": \"integer\",\n      \"description\": \"Task type identifier (0=ReloadTask)\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the task is enabled for execution\",\n      \"default\": true\n    },\n    \"taskSessionTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum execution time in minutes before the task is terminated\",\n      \"minimum\": 0\n    },\n    \"maxRetries\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of automatic retry attempts on failure\",\n      \"minimum\": 0,\n      \"default\": 0\n    },\n    \"app\": {\n      \"$ref\": \"#/$defs/AppReference\"\
  ,\n      \"description\": \"The application this reload task is associated with\"\n    },\n    \"isManuallyTriggered\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the task requires manual triggering rather than scheduled execution\",\n      \"default\": false\n    },\n    \"operational\": {\n      \"$ref\": \"#/$defs/TaskOperational\",\n      \"description\": \"Operational information including last execution result and next execution time\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TagReference\"\n      },\n      \"description\": \"Tags applied to the task\"\n    },\n    \"customProperties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomPropertyValue\"\n      },\n      \"description\": \"Custom property values assigned to the task\"\n    },\n    \"privileges\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\"\
  : \"List of privileges the current user has on this task\"\n    },\n    \"schemaPath\": {\n      \"type\": \"string\",\n      \"description\": \"Schema path identifying the entity type in the QRS\"\n    }\n  },\n  \"required\": [\"name\"],\n  \"$defs\": {\n    \"AppReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"appId\": {\n          \"type\": \"string\"\n        },\n        \"publishTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"published\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"TaskOperational\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"lastExecutionResult\": {\n          \"$ref\": \"#/$defs/ExecutionResult\"\
  \n        },\n        \"nextExecution\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Scheduled time of the next execution\"\n        }\n      }\n    },\n    \"ExecutionResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"executingNodeName\": {\n          \"type\": \"string\",\n          \"description\": \"Hostname of the node that executed the task\"\n        },\n        \"status\": {\n          \"type\": \"integer\",\n          \"description\": \"Execution status code\",\n          \"enum\": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]\n        },\n        \"startTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the execution started\"\n        },\n        \"stopTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n  \
  \        \"description\": \"When the execution completed\"\n        },\n        \"duration\": {\n          \"type\": \"integer\",\n          \"description\": \"Execution duration in milliseconds\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"TagReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"CustomPropertyValue\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"definition\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"format\": \"uuid\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n      \
  \  \"value\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/json-schema/qlik-sense-enterprise-reload-task-schema.json
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Enterprise
- REST API
title: Qlik Sense Reload Task
---
