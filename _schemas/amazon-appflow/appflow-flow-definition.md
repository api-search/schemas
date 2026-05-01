---
description: FlowDefinition schema from Amazon AppFlow API
layout: schema
name: FlowDefinition
properties_list:
- description: The flow's Amazon Resource Name (ARN).
  name: flowArn
  type: string
- description: A user-entered description of the flow.
  name: description
  type: string
- description: The specified name of the flow.
  name: flowName
  type: string
- description: Indicates the current status of the flow.
  name: flowStatus
  type: string
- description: Specifies the source connector type.
  name: sourceConnectorType
  type: string
- description: The label of the source connector in the flow.
  name: sourceConnectorLabel
  type: string
- description: Specifies the destination connector type.
  name: destinationConnectorType
  type: string
- description: The label of the destination connector in the flow.
  name: destinationConnectorLabel
  type: string
- description: Specifies the type of flow trigger.
  name: triggerType
  type: string
- description: Specifies when the flow was created.
  name: createdAt
  type: integer
- description: Specifies when the flow was last updated.
  name: lastUpdatedAt
  type: integer
- description: The ARN of the user who created the flow.
  name: createdBy
  type: string
- description: Specifies the account user name that most recently updated the flow.
  name: lastUpdatedBy
  type: string
- description: ''
  name: tags
  type: object
- description: ''
  name: lastRunExecutionDetails
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-flow-definition-schema.json
slug: appflow-flow-definition
source_filename: appflow-flow-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-flow-definition-schema.json\",\n  \"title\": \"FlowDefinition\",\n  \"description\": \"FlowDefinition schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flowArn\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:appflow:us-east-1:123456789012:flow/my-salesforce-to-s3-flow\",\n      \"description\": \"The flow's Amazon Resource Name (ARN).\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Transfer Salesforce accounts to S3 daily\",\n      \"description\": \"A user-entered description of the flow.\"\n    },\n    \"flowName\": {\n      \"type\": \"string\",\n      \"example\": \"my-salesforce-to-s3-flow\",\n      \"description\": \"The specified name of the flow.\"\n    },\n    \"flowStatus\": {\n      \"type\": \"\
  string\",\n      \"enum\": [\n        \"Active\",\n        \"Deprecated\",\n        \"Deleted\",\n        \"Draft\",\n        \"Errored\",\n        \"Suspended\"\n      ],\n      \"example\": \"Active\",\n      \"description\": \"Indicates the current status of the flow.\"\n    },\n    \"sourceConnectorType\": {\n      \"type\": \"string\",\n      \"example\": \"Salesforce\",\n      \"description\": \"Specifies the source connector type.\"\n    },\n    \"sourceConnectorLabel\": {\n      \"type\": \"string\",\n      \"example\": \"MyCustomSourceConnector\",\n      \"description\": \"The label of the source connector in the flow.\"\n    },\n    \"destinationConnectorType\": {\n      \"type\": \"string\",\n      \"example\": \"S3\",\n      \"description\": \"Specifies the destination connector type.\"\n    },\n    \"destinationConnectorLabel\": {\n      \"type\": \"string\",\n      \"example\": \"MyCustomDestinationConnector\",\n      \"description\": \"The label of the destination connector\
  \ in the flow.\"\n    },\n    \"triggerType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Scheduled\",\n        \"Event\",\n        \"OnDemand\"\n      ],\n      \"example\": \"Scheduled\",\n      \"description\": \"Specifies the type of flow trigger.\"\n    },\n    \"createdAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993,\n      \"description\": \"Specifies when the flow was created.\"\n    },\n    \"lastUpdatedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993,\n      \"description\": \"Specifies when the flow was last updated.\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:iam::123456789012:user/admin\",\n      \"description\": \"The ARN of the user who created the flow.\"\n    },\n    \"lastUpdatedBy\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:iam::123456789012:user/admin\",\n      \"description\"\
  : \"Specifies the account user name that most recently updated the flow.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"environment\": \"production\"\n      }\n    },\n    \"lastRunExecutionDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"mostRecentExecutionMessage\": {\n          \"type\": \"string\",\n          \"example\": \"Successfully ran the flow\",\n          \"description\": \"Describes the details of the most recent flow run.\"\n        },\n        \"mostRecentExecutionTime\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"example\": 1718153700000,\n          \"description\": \"Specifies the time of the most recent flow run.\"\n        },\n        \"mostRecentExecutionStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"InProgress\",\n            \"Successful\",\n   \
  \         \"Error\",\n            \"CancelStarted\",\n            \"Canceled\"\n          ],\n          \"example\": \"Successful\",\n          \"description\": \"Specifies the status of the most recent flow run.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-flow-definition-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: FlowDefinition
---
