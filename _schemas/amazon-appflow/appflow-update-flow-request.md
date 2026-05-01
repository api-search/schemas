---
description: UpdateFlowRequest schema from Amazon AppFlow API
layout: schema
name: UpdateFlowRequest
properties_list:
- description: The specified name of the flow.
  name: flowName
  type: string
- description: Idempotency token.
  name: clientToken
  type: string
- description: A description of the flow.
  name: description
  type: string
- description: ''
  name: triggerConfig
  type: object
- description: ''
  name: sourceFlowConfig
  type: object
- description: ''
  name: destinationFlowConfigList
  type: array
- description: ''
  name: tasks
  type: array
- description: ''
  name: metadataCatalogConfig
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-update-flow-request-schema.json
slug: appflow-update-flow-request
source_filename: appflow-update-flow-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-update-flow-request-schema.json\",\n  \"title\": \"UpdateFlowRequest\",\n  \"description\": \"UpdateFlowRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flowName\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"my-salesforce-to-s3-flow\",\n      \"description\": \"The specified name of the flow.\"\n    },\n    \"clientToken\": {\n      \"type\": \"string\",\n      \"example\": \"client-token-500123\",\n      \"description\": \"Idempotency token.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"maxLength\": 2048,\n      \"example\": \"Updated description\",\n      \"description\": \"A description of the flow.\"\n    },\n    \"triggerConfig\": {\n      \"type\": \"object\",\n      \"properties\"\
  : {\n        \"triggerType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Scheduled\",\n            \"Event\",\n            \"OnDemand\"\n          ],\n          \"example\": \"Scheduled\",\n          \"description\": \"Specifies the type of flow trigger. It can be OnDemand, Scheduled, or Event.\"\n        },\n        \"triggerProperties\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Scheduled\": {}\n          },\n          \"description\": \"Specifies the configuration details of a schedule-triggered flow as defined by the user.\"\n        }\n      },\n      \"required\": [\n        \"triggerType\"\n      ]\n    },\n    \"sourceFlowConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"connectorType\": {\n          \"type\": \"string\",\n          \"example\": \"Salesforce\",\n          \"description\": \"The type of connector used as a source.\"\n        },\n        \"apiVersion\": {\n          \"type\"\
  : \"string\",\n          \"example\": \"v55.0\",\n          \"description\": \"The API version of the connector used in the source.\"\n        },\n        \"connectorProfileName\": {\n          \"type\": \"string\",\n          \"example\": \"my-salesforce-profile\",\n          \"description\": \"The name of the connector profile. Required for all connectors except Amplitude, Datadog, Dynatrace, GoogleAnalytics, Marketo, SAPOData, Salesforce, ServiceNow, Singular, Slack, Trendmicro, and Veeva.\"\n        },\n        \"sourceConnectorProperties\": {\n          \"type\": \"object\",\n          \"example\": {\n            \"Salesforce\": {\n              \"object\": \"Account\"\n            }\n          },\n          \"description\": \"Specifies the information that is required to query a particular source connector.\"\n        },\n        \"incrementalPullConfig\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"datetimeTypeFieldName\": {\n              \"type\"\
  : \"string\",\n              \"example\": \"LastModifiedDate\",\n              \"description\": \"A field that specifies the date time or timestamp field as the criteria to use when importing incremental records from the source.\"\n            }\n          },\n          \"description\": \"Defines the configuration for a scheduled incremental data pull. If a valid configuration is provided, the fields specified in the configuration are used when querying for the incremental data pull.\"\n        }\n      },\n      \"required\": [\n        \"connectorType\",\n        \"sourceConnectorProperties\"\n      ]\n    },\n    \"destinationFlowConfigList\": {\n      \"type\": \"array\",\n      \"items\": {}\n    },\n    \"tasks\": {\n      \"type\": \"array\",\n      \"items\": {}\n    },\n    \"metadataCatalogConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"glueDataCatalog\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"roleArn\": {\n\
  \              \"type\": \"string\",\n              \"example\": \"arn:aws:iam::123456789012:role/AppFlowGlueRole\",\n              \"description\": \"The ARN of an IAM role that grants AppFlow the permissions it needs to create Data Catalog tables, databases, and partitions.\"\n            },\n            \"databaseName\": {\n              \"type\": \"string\",\n              \"example\": \"appflow-catalog-db\",\n              \"description\": \"The name of an existing Glue Data Catalog database.\"\n            },\n            \"tablePrefix\": {\n              \"type\": \"string\",\n              \"example\": \"sf_\",\n              \"description\": \"A naming prefix for each Data Catalog table that Amazon AppFlow creates.\"\n            }\n          },\n          \"description\": \"Specifies the configuration that Amazon AppFlow uses when it catalogs data with the Glue Data Catalog.\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"flowName\",\n    \"triggerConfig\",\n   \
  \ \"sourceFlowConfig\",\n    \"destinationFlowConfigList\",\n    \"tasks\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-update-flow-request-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: UpdateFlowRequest
---
