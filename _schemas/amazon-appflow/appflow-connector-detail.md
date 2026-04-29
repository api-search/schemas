---
description: ConnectorDetail schema from Amazon AppFlow API
layout: schema
name: ConnectorDetail
properties_list:
- description: A description about the registered connector.
  name: connectorDescription
  type: string
- description: The name of the connector.
  name: connectorName
  type: string
- description: The owner of the connector.
  name: connectorOwner
  type: string
- description: The connector version.
  name: connectorVersion
  type: string
- description: The application type of the connector.
  name: applicationType
  type: string
- description: The connector type.
  name: connectorType
  type: string
- description: The label used for registering the connector.
  name: connectorLabel
  type: string
- description: The time at which the connector was registered.
  name: registeredAt
  type: integer
- description: The user who registered the connector.
  name: registeredBy
  type: string
- description: The provisioning type that the connector uses.
  name: connectorProvisioningType
  type: string
- description: ''
  name: connectorModes
  type: array
- description: ''
  name: supportedDataTransferTypes
  type: array
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-connector-detail-schema.json
slug: appflow-connector-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-connector-detail-schema.json\",\n  \"title\": \"ConnectorDetail\",\n  \"description\": \"ConnectorDetail schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorDescription\": {\n      \"type\": \"string\",\n      \"example\": \"My custom connector for proprietary data source\",\n      \"description\": \"A description about the registered connector.\"\n    },\n    \"connectorName\": {\n      \"type\": \"string\",\n      \"example\": \"MyCustomConnector\",\n      \"description\": \"The name of the connector.\"\n    },\n    \"connectorOwner\": {\n      \"type\": \"string\",\n      \"example\": \"123456789012\",\n      \"description\": \"The owner of the connector.\"\n    },\n    \"connectorVersion\": {\n      \"type\": \"string\",\n      \"example\": \"1.0\"\
  ,\n      \"description\": \"The connector version.\"\n    },\n    \"applicationType\": {\n      \"type\": \"string\",\n      \"example\": \"SaaS\",\n      \"description\": \"The application type of the connector.\"\n    },\n    \"connectorType\": {\n      \"type\": \"string\",\n      \"example\": \"CustomConnector\",\n      \"description\": \"The connector type.\"\n    },\n    \"connectorLabel\": {\n      \"type\": \"string\",\n      \"example\": \"MyCustomConnector\",\n      \"description\": \"The label used for registering the connector.\"\n    },\n    \"registeredAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993,\n      \"description\": \"The time at which the connector was registered.\"\n    },\n    \"registeredBy\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:iam::123456789012:user/admin\",\n      \"description\": \"The user who registered the connector.\"\n    },\n    \"connectorProvisioningType\": {\n      \"type\"\
  : \"string\",\n      \"example\": \"LAMBDA\",\n      \"description\": \"The provisioning type that the connector uses.\"\n    },\n    \"connectorModes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"example\": \"\"\n      },\n      \"example\": [\n        \"CLOUD\"\n      ]\n    },\n    \"supportedDataTransferTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"example\": \"\"\n      },\n      \"example\": [\n        \"RECORD\",\n        \"FILE\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-connector-detail-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ConnectorDetail
---
