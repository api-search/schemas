---
description: Schema defining the structure of an Amazon AppFlow flow resource, including source and destination configurations, task definitions, trigger settings, and flow metadata.
layout: schema
name: Amazon AppFlow Flow Definition
properties_list:
- description: The ARN of the flow.
  name: flowArn
  type: string
- description: The specified name of the flow.
  name: flowName
  type: string
- description: A user-entered description of the flow.
  name: description
  type: string
- description: Indicates the current status of the flow.
  name: flowStatus
  type: string
- description: ''
  name: sourceFlowConfig
  type: object
- description: The configuration that controls how Amazon AppFlow places data in the destination connector.
  name: destinationFlowConfigList
  type: array
- description: A list of tasks that Amazon AppFlow performs while transferring the data in the flow run.
  name: tasks
  type: array
- description: ''
  name: triggerConfig
  type: object
- description: Specifies when the flow was created.
  name: createdAt
  type: string
- description: Specifies when the flow was last updated.
  name: lastUpdatedAt
  type: string
- description: The tags used to organize, track, or control access for your flow.
  name: tags
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/amazon-appflow-schema.json
slug: amazon-appflow
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apievangelist.com/amazon-appflow/flow-definition\",\n  \"title\": \"Amazon AppFlow Flow Definition\",\n  \"description\": \"Schema defining the structure of an Amazon AppFlow flow resource, including source and destination configurations, task definitions, trigger settings, and flow metadata.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"flowName\",\n    \"sourceFlowConfig\",\n    \"destinationFlowConfigList\",\n    \"tasks\",\n    \"triggerConfig\"\n  ],\n  \"properties\": {\n    \"flowArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the flow.\"\n    },\n    \"flowName\": {\n      \"type\": \"string\",\n      \"description\": \"The specified name of the flow.\",\n      \"pattern\": \"^[a-zA-Z0-9][a-zA-Z0-9_-]*$\",\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A user-entered description\
  \ of the flow.\",\n      \"maxLength\": 2048\n    },\n    \"flowStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Deprecated\",\n        \"Deleted\",\n        \"Draft\",\n        \"Errored\",\n        \"Suspended\"\n      ],\n      \"description\": \"Indicates the current status of the flow.\"\n    },\n    \"sourceFlowConfig\": {\n      \"$ref\": \"#/$defs/SourceFlowConfig\"\n    },\n    \"destinationFlowConfigList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DestinationFlowConfig\"\n      },\n      \"description\": \"The configuration that controls how Amazon AppFlow places data in the destination connector.\"\n    },\n    \"tasks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Task\"\n      },\n      \"description\": \"A list of tasks that Amazon AppFlow performs while transferring the data in the flow run.\"\n    },\n    \"triggerConfig\": {\n      \"$ref\": \"#/$defs/TriggerConfig\"\
  \n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Specifies when the flow was created.\"\n    },\n    \"lastUpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Specifies when the flow was last updated.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The tags used to organize, track, or control access for your flow.\"\n    }\n  },\n  \"$defs\": {\n    \"SourceFlowConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Contains information about the configuration of the source connector.\",\n      \"required\": [\n        \"connectorType\",\n        \"sourceConnectorProperties\"\n      ],\n      \"properties\": {\n        \"connectorType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of connector, such as Salesforce, Zendesk,\
  \ Slack, etc.\"\n        },\n        \"connectorProfileName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the connector profile.\"\n        },\n        \"sourceConnectorProperties\": {\n          \"type\": \"object\",\n          \"description\": \"Specifies the information that is required to query a particular source connector.\"\n        },\n        \"incrementalPullConfig\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"datetimeTypeFieldName\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"DestinationFlowConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Contains information about the configuration of destination connector.\",\n      \"required\": [\n        \"connectorType\",\n        \"destinationConnectorProperties\"\n      ],\n      \"properties\": {\n        \"connectorType\": {\n          \"type\": \"string\",\n          \"description\": \"\
  The type of destination connector.\"\n        },\n        \"connectorProfileName\": {\n          \"type\": \"string\"\n        },\n        \"destinationConnectorProperties\": {\n          \"type\": \"object\",\n          \"description\": \"The properties that are required to query the destination connector.\"\n        }\n      }\n    },\n    \"Task\": {\n      \"type\": \"object\",\n      \"description\": \"A class for modeling different type of tasks.\",\n      \"required\": [\n        \"sourceFields\",\n        \"taskType\"\n      ],\n      \"properties\": {\n        \"sourceFields\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"The source fields to which a particular task is applied.\"\n        },\n        \"connectorOperator\": {\n          \"type\": \"object\",\n          \"description\": \"The operation to be performed on the provided source fields.\"\n        },\n        \"destinationField\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"A field in a destination connector.\"\n        },\n        \"taskType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Arithmetic\",\n            \"Filter\",\n            \"Map\",\n            \"Map_all\",\n            \"Mask\",\n            \"Merge\",\n            \"Passthrough\",\n            \"Truncate\",\n            \"Validate\",\n            \"Partition\"\n          ],\n          \"description\": \"Specifies the particular task implementation.\"\n        },\n        \"taskProperties\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"TriggerConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The trigger settings that determine how and when Amazon AppFlow runs the specified flow.\",\n      \"required\": [\n        \"triggerType\"\n      ],\n      \"properties\": {\n  \
  \      \"triggerType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Scheduled\",\n            \"Event\",\n            \"OnDemand\"\n          ],\n          \"description\": \"Specifies the type of flow trigger.\"\n        },\n        \"triggerProperties\": {\n          \"type\": \"object\",\n          \"description\": \"Specifies the configuration details of a schedule-triggered flow.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/amazon-appflow-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: Amazon AppFlow Flow Definition
---
