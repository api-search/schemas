---
description: CreateFlowRequest schema from Amazon AppFlow API
layout: schema
name: CreateFlowRequest
properties_list:
- description: The specified name of the flow. Spaces are not allowed. Use underscores or hyphens only.
  name: flowName
  type: string
- description: Idempotency token to ensure CreateFlow completes only once.
  name: clientToken
  type: string
- description: A description of the flow you want to create.
  name: description
  type: string
- description: The ARN of the KMS key for encryption.
  name: kmsArn
  type: string
- description: ''
  name: metadataCatalogConfig
  type: object
- description: ''
  name: triggerConfig
  type: object
- description: ''
  name: sourceFlowConfig
  type: object
- description: The configuration that controls how Amazon AppFlow places data in the destination connector.
  name: destinationFlowConfigList
  type: array
- description: A list of tasks that Amazon AppFlow performs while transferring data in the flow run.
  name: tasks
  type: array
- description: The tags used to organize, track, or control access for your flow.
  name: tags
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-create-flow-request-schema.json
slug: appflow-create-flow-request
source_filename: appflow-create-flow-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-create-flow-request-schema.json\",\n  \"title\": \"CreateFlowRequest\",\n  \"description\": \"CreateFlowRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flowName\": {\n      \"type\": \"string\",\n      \"pattern\": \"[a-zA-Z0-9][\\\\w!@#.-]+\",\n      \"maxLength\": 256,\n      \"example\": \"my-salesforce-to-s3-flow\",\n      \"description\": \"The specified name of the flow. Spaces are not allowed. Use underscores or hyphens only.\"\n    },\n    \"clientToken\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 256,\n      \"example\": \"client-token-500123\",\n      \"description\": \"Idempotency token to ensure CreateFlow completes only once.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"maxLength\"\
  : 2048,\n      \"example\": \"Transfer Salesforce accounts to S3 daily\",\n      \"description\": \"A description of the flow you want to create.\"\n    },\n    \"kmsArn\": {\n      \"type\": \"string\",\n      \"minLength\": 20,\n      \"maxLength\": 2048,\n      \"example\": \"arn:aws:kms:us-east-1:123456789012:key/mrk-1234abcd\",\n      \"description\": \"The ARN of the KMS key for encryption.\"\n    },\n    \"metadataCatalogConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"glueDataCatalog\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"roleArn\": {\n              \"type\": \"string\",\n              \"example\": \"arn:aws:iam::123456789012:role/AppFlowGlueRole\",\n              \"description\": \"The ARN of an IAM role that grants AppFlow the permissions it needs to create Data Catalog tables, databases, and partitions.\"\n            },\n            \"databaseName\": {\n              \"type\": \"string\",\n             \
  \ \"example\": \"appflow-catalog-db\",\n              \"description\": \"The name of an existing Glue Data Catalog database.\"\n            },\n            \"tablePrefix\": {\n              \"type\": \"string\",\n              \"example\": \"sf_\",\n              \"description\": \"A naming prefix for each Data Catalog table that Amazon AppFlow creates.\"\n            }\n          },\n          \"description\": \"Specifies the configuration that Amazon AppFlow uses when it catalogs data with the Glue Data Catalog.\"\n        }\n      }\n    },\n    \"triggerConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"triggerType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Scheduled\",\n            \"Event\",\n            \"OnDemand\"\n          ],\n          \"example\": \"Scheduled\",\n          \"description\": \"Specifies the type of flow trigger. It can be OnDemand, Scheduled, or Event.\"\n        },\n        \"triggerProperties\": {\n\
  \          \"type\": \"object\",\n          \"properties\": {\n            \"Scheduled\": {}\n          },\n          \"description\": \"Specifies the configuration details of a schedule-triggered flow as defined by the user.\"\n        }\n      },\n      \"required\": [\n        \"triggerType\"\n      ]\n    },\n    \"sourceFlowConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"connectorType\": {\n          \"type\": \"string\",\n          \"example\": \"Salesforce\",\n          \"description\": \"The type of connector used as a source.\"\n        },\n        \"apiVersion\": {\n          \"type\": \"string\",\n          \"example\": \"v55.0\",\n          \"description\": \"The API version of the connector used in the source.\"\n        },\n        \"connectorProfileName\": {\n          \"type\": \"string\",\n          \"example\": \"my-salesforce-profile\",\n          \"description\": \"The name of the connector profile. Required for all connectors except Amplitude,\
  \ Datadog, Dynatrace, GoogleAnalytics, Marketo, SAPOData, Salesforce, ServiceNow, Singular, Slack, Trendmicro, and Veeva.\"\n        },\n        \"sourceConnectorProperties\": {\n          \"type\": \"object\",\n          \"example\": {\n            \"Salesforce\": {\n              \"object\": \"Account\"\n            }\n          },\n          \"description\": \"Specifies the information that is required to query a particular source connector.\"\n        },\n        \"incrementalPullConfig\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"datetimeTypeFieldName\": {\n              \"type\": \"string\",\n              \"example\": \"LastModifiedDate\",\n              \"description\": \"A field that specifies the date time or timestamp field as the criteria to use when importing incremental records from the source.\"\n            }\n          },\n          \"description\": \"Defines the configuration for a scheduled incremental data pull. If a valid configuration\
  \ is provided, the fields specified in the configuration are used when querying for the incremental data pull.\"\n        }\n      },\n      \"required\": [\n        \"connectorType\",\n        \"sourceConnectorProperties\"\n      ]\n    },\n    \"destinationFlowConfigList\": {\n      \"type\": \"array\",\n      \"items\": {},\n      \"description\": \"The configuration that controls how Amazon AppFlow places data in the destination connector.\"\n    },\n    \"tasks\": {\n      \"type\": \"array\",\n      \"items\": {},\n      \"description\": \"A list of tasks that Amazon AppFlow performs while transferring data in the flow run.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"environment\": \"production\"\n      },\n      \"description\": \"The tags used to organize, track, or control access for your flow.\"\n    }\n  },\n  \"required\": [\n    \"flowName\",\n    \"triggerConfig\"\
  ,\n    \"sourceFlowConfig\",\n    \"destinationFlowConfigList\",\n    \"tasks\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-create-flow-request-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: CreateFlowRequest
---
