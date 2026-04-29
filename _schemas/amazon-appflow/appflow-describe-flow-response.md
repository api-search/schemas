---
description: DescribeFlowResponse schema from Amazon AppFlow API
layout: schema
name: DescribeFlowResponse
properties_list:
- description: The flow's Amazon Resource Name (ARN).
  name: flowArn
  type: string
- description: A description of the flow.
  name: description
  type: string
- description: The specified name of the flow.
  name: flowName
  type: string
- description: The ARN of the AWS KMS key.
  name: kmsArn
  type: string
- description: Indicates the current status of the flow.
  name: flowStatus
  type: string
- description: Contains an error message if the flow status is in a suspended or error state.
  name: flowStatusMessage
  type: string
- description: ''
  name: sourceFlowConfig
  type: object
- description: ''
  name: destinationFlowConfigList
  type: array
- description: ''
  name: lastRunExecutionDetails
  type: object
- description: ''
  name: triggerConfig
  type: object
- description: ''
  name: tasks
  type: array
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
  name: metadataCatalogConfig
  type: object
- description: ''
  name: lastRunMetadataCatalogDetails
  type: array
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-describe-flow-response-schema.json
slug: appflow-describe-flow-response
source_filename: appflow-describe-flow-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-flow-response-schema.json\",\n  \"title\": \"DescribeFlowResponse\",\n  \"description\": \"DescribeFlowResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flowArn\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:appflow:us-east-1:123456789012:flow/my-salesforce-to-s3-flow\",\n      \"description\": \"The flow's Amazon Resource Name (ARN).\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Transfer Salesforce accounts to S3 daily\",\n      \"description\": \"A description of the flow.\"\n    },\n    \"flowName\": {\n      \"type\": \"string\",\n      \"example\": \"my-salesforce-to-s3-flow\",\n      \"description\": \"The specified name of the flow.\"\n    },\n    \"kmsArn\": {\n      \"type\": \"\
  string\",\n      \"example\": \"arn:aws:kms:us-east-1:123456789012:key/mrk-1234abcd\",\n      \"description\": \"The ARN of the AWS KMS key.\"\n    },\n    \"flowStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Deprecated\",\n        \"Deleted\",\n        \"Draft\",\n        \"Errored\",\n        \"Suspended\"\n      ],\n      \"example\": \"Active\",\n      \"description\": \"Indicates the current status of the flow.\"\n    },\n    \"flowStatusMessage\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"Contains an error message if the flow status is in a suspended or error state.\"\n    },\n    \"sourceFlowConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"connectorType\": {\n          \"type\": \"string\",\n          \"example\": \"Salesforce\",\n          \"description\": \"The type of connector used as a source.\"\n        },\n        \"apiVersion\": {\n          \"type\": \"string\"\
  ,\n          \"example\": \"v55.0\",\n          \"description\": \"The API version of the connector used in the source.\"\n        },\n        \"connectorProfileName\": {\n          \"type\": \"string\",\n          \"example\": \"my-salesforce-profile\",\n          \"description\": \"The name of the connector profile. Required for all connectors except Amplitude, Datadog, Dynatrace, GoogleAnalytics, Marketo, SAPOData, Salesforce, ServiceNow, Singular, Slack, Trendmicro, and Veeva.\"\n        },\n        \"sourceConnectorProperties\": {\n          \"type\": \"object\",\n          \"example\": {\n            \"Salesforce\": {\n              \"object\": \"Account\"\n            }\n          },\n          \"description\": \"Specifies the information that is required to query a particular source connector.\"\n        },\n        \"incrementalPullConfig\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"datetimeTypeFieldName\": {\n              \"type\": \"string\"\
  ,\n              \"example\": \"LastModifiedDate\",\n              \"description\": \"A field that specifies the date time or timestamp field as the criteria to use when importing incremental records from the source.\"\n            }\n          },\n          \"description\": \"Defines the configuration for a scheduled incremental data pull. If a valid configuration is provided, the fields specified in the configuration are used when querying for the incremental data pull.\"\n        }\n      },\n      \"required\": [\n        \"connectorType\",\n        \"sourceConnectorProperties\"\n      ]\n    },\n    \"destinationFlowConfigList\": {\n      \"type\": \"array\",\n      \"items\": {}\n    },\n    \"lastRunExecutionDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"mostRecentExecutionMessage\": {\n          \"type\": \"string\",\n          \"example\": \"Successfully ran the flow\",\n          \"description\": \"Describes the details of the most recent flow run.\"\
  \n        },\n        \"mostRecentExecutionTime\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"example\": 1718153700000,\n          \"description\": \"Specifies the time of the most recent flow run.\"\n        },\n        \"mostRecentExecutionStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"InProgress\",\n            \"Successful\",\n            \"Error\",\n            \"CancelStarted\",\n            \"Canceled\"\n          ],\n          \"example\": \"Successful\",\n          \"description\": \"Specifies the status of the most recent flow run.\"\n        }\n      }\n    },\n    \"triggerConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"triggerType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Scheduled\",\n            \"Event\",\n            \"OnDemand\"\n          ],\n          \"example\": \"Scheduled\",\n          \"description\": \"Specifies the type of\
  \ flow trigger. It can be OnDemand, Scheduled, or Event.\"\n        },\n        \"triggerProperties\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Scheduled\": {}\n          },\n          \"description\": \"Specifies the configuration details of a schedule-triggered flow as defined by the user.\"\n        }\n      },\n      \"required\": [\n        \"triggerType\"\n      ]\n    },\n    \"tasks\": {\n      \"type\": \"array\",\n      \"items\": {}\n    },\n    \"createdAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993,\n      \"description\": \"Specifies when the flow was created.\"\n    },\n    \"lastUpdatedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993,\n      \"description\": \"Specifies when the flow was last updated.\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:iam::123456789012:user/admin\",\n  \
  \    \"description\": \"The ARN of the user who created the flow.\"\n    },\n    \"lastUpdatedBy\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:iam::123456789012:user/admin\",\n      \"description\": \"Specifies the account user name that most recently updated the flow.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"environment\": \"production\"\n      }\n    },\n    \"metadataCatalogConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"glueDataCatalog\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"roleArn\": {\n              \"type\": \"string\",\n              \"example\": \"arn:aws:iam::123456789012:role/AppFlowGlueRole\",\n              \"description\": \"The ARN of an IAM role that grants AppFlow the permissions it needs to create Data Catalog tables, databases, and partitions.\"\n          \
  \  },\n            \"databaseName\": {\n              \"type\": \"string\",\n              \"example\": \"appflow-catalog-db\",\n              \"description\": \"The name of an existing Glue Data Catalog database.\"\n            },\n            \"tablePrefix\": {\n              \"type\": \"string\",\n              \"example\": \"sf_\",\n              \"description\": \"A naming prefix for each Data Catalog table that Amazon AppFlow creates.\"\n            }\n          },\n          \"description\": \"Specifies the configuration that Amazon AppFlow uses when it catalogs data with the Glue Data Catalog.\"\n        }\n      }\n    },\n    \"lastRunMetadataCatalogDetails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-flow-response-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: DescribeFlowResponse
---
