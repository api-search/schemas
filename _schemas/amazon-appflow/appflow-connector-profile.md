---
description: ConnectorProfile schema from Amazon AppFlow API
layout: schema
name: ConnectorProfile
properties_list:
- description: The Amazon Resource Name (ARN) of the connector profile.
  name: connectorProfileArn
  type: string
- description: The name of the connector profile.
  name: connectorProfileName
  type: string
- description: The type of connector.
  name: connectorType
  type: string
- description: The label of the connector.
  name: connectorLabel
  type: string
- description: Indicates the connection mode and if it is public or private.
  name: connectionMode
  type: string
- description: The Amazon Resource Name (ARN) of the connector profile credentials.
  name: credentialsArn
  type: string
- description: The connector-specific properties of the profile configuration.
  name: connectorProfileProperties
  type: object
- description: Specifies when the connector profile was created.
  name: createdAt
  type: integer
- description: Specifies when the connector profile was last updated.
  name: lastUpdatedAt
  type: integer
- description: Specifies the private connection provisioning state.
  name: privateConnectionProvisioningState
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-connector-profile-schema.json
slug: appflow-connector-profile
source_filename: appflow-connector-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-connector-profile-schema.json\",\n  \"title\": \"ConnectorProfile\",\n  \"description\": \"ConnectorProfile schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorProfileArn\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:appflow:us-east-1:123456789012:connectorprofile/my-salesforce-profile\",\n      \"description\": \"The Amazon Resource Name (ARN) of the connector profile.\"\n    },\n    \"connectorProfileName\": {\n      \"type\": \"string\",\n      \"example\": \"my-salesforce-profile\",\n      \"description\": \"The name of the connector profile.\"\n    },\n    \"connectorType\": {\n      \"type\": \"string\",\n      \"example\": \"Salesforce\",\n      \"description\": \"The type of connector.\"\n    },\n    \"connectorLabel\": {\n  \
  \    \"type\": \"string\",\n      \"example\": \"MyCustomConnector\",\n      \"description\": \"The label of the connector.\"\n    },\n    \"connectionMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Public\",\n        \"Private\"\n      ],\n      \"example\": \"Public\",\n      \"description\": \"Indicates the connection mode and if it is public or private.\"\n    },\n    \"credentialsArn\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:secretsmanager:us-east-1:123456789012:secret:appflow/my-salesforce-profile-credentials\",\n      \"description\": \"The Amazon Resource Name (ARN) of the connector profile credentials.\"\n    },\n    \"connectorProfileProperties\": {\n      \"type\": \"object\",\n      \"description\": \"The connector-specific properties of the profile configuration.\"\n    },\n    \"createdAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993,\n      \"description\": \"Specifies when the\
  \ connector profile was created.\"\n    },\n    \"lastUpdatedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993,\n      \"description\": \"Specifies when the connector profile was last updated.\"\n    },\n    \"privateConnectionProvisioningState\": {\n      \"type\": \"object\",\n      \"description\": \"Specifies the private connection provisioning state.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-connector-profile-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ConnectorProfile
---
