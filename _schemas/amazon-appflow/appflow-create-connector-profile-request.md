---
description: CreateConnectorProfileRequest schema from Amazon AppFlow API
layout: schema
name: CreateConnectorProfileRequest
properties_list:
- description: The name of the connector profile. The name is unique for each ConnectorProfile in your AWS account.
  name: connectorProfileName
  type: string
- description: Idempotency token.
  name: clientToken
  type: string
- description: The type of connector, such as Salesforce, Marketo, and so on.
  name: connectorType
  type: string
- description: The label of the connector. The label is unique for each ConnectorRegistration in your AWS account.
  name: connectorLabel
  type: string
- description: Indicates the connection mode and specifies whether it is public or private.
  name: connectionMode
  type: string
- description: The ARN of the KMS key to use to encrypt your connector profile credentials.
  name: kmsArn
  type: string
- description: Defines the connector-specific configuration and credentials.
  name: connectorProfileConfig
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-create-connector-profile-request-schema.json
slug: appflow-create-connector-profile-request
source_filename: appflow-create-connector-profile-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-create-connector-profile-request-schema.json\",\n  \"title\": \"CreateConnectorProfileRequest\",\n  \"description\": \"CreateConnectorProfileRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorProfileName\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"my-salesforce-profile\",\n      \"description\": \"The name of the connector profile. The name is unique for each ConnectorProfile in your AWS account.\"\n    },\n    \"clientToken\": {\n      \"type\": \"string\",\n      \"example\": \"client-token-500123\",\n      \"description\": \"Idempotency token.\"\n    },\n    \"connectorType\": {\n      \"type\": \"string\",\n      \"example\": \"Salesforce\",\n      \"description\": \"The type of connector, such as Salesforce,\
  \ Marketo, and so on.\"\n    },\n    \"connectorLabel\": {\n      \"type\": \"string\",\n      \"example\": \"MyCustomConnector\",\n      \"description\": \"The label of the connector. The label is unique for each ConnectorRegistration in your AWS account.\"\n    },\n    \"connectionMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Public\",\n        \"Private\"\n      ],\n      \"example\": \"Public\",\n      \"description\": \"Indicates the connection mode and specifies whether it is public or private.\"\n    },\n    \"kmsArn\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:kms:us-east-1:123456789012:key/mrk-1234abcd\",\n      \"description\": \"The ARN of the KMS key to use to encrypt your connector profile credentials.\"\n    },\n    \"connectorProfileConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Defines the connector-specific configuration and credentials.\"\n    }\n  },\n  \"required\": [\n    \"connectorProfileName\",\n    \"\
  connectorType\",\n    \"connectionMode\",\n    \"connectorProfileConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-create-connector-profile-request-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: CreateConnectorProfileRequest
---
