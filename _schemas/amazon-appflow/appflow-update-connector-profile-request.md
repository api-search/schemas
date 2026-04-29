---
description: UpdateConnectorProfileRequest schema from Amazon AppFlow API
layout: schema
name: UpdateConnectorProfileRequest
properties_list:
- description: The name of the connector profile and is unique for each ConnectorProfile in the AWS account.
  name: connectorProfileName
  type: string
- description: Idempotency token.
  name: clientToken
  type: string
- description: Indicates the connection mode and if it is public or private.
  name: connectionMode
  type: string
- description: Defines the connector-specific profile configuration and credentials.
  name: connectorProfileConfig
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-update-connector-profile-request-schema.json
slug: appflow-update-connector-profile-request
source_filename: appflow-update-connector-profile-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-update-connector-profile-request-schema.json\",\n  \"title\": \"UpdateConnectorProfileRequest\",\n  \"description\": \"UpdateConnectorProfileRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorProfileName\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"my-salesforce-profile\",\n      \"description\": \"The name of the connector profile and is unique for each ConnectorProfile in the AWS account.\"\n    },\n    \"clientToken\": {\n      \"type\": \"string\",\n      \"example\": \"client-token-500123\",\n      \"description\": \"Idempotency token.\"\n    },\n    \"connectionMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Public\",\n        \"Private\"\n      ],\n      \"example\": \"Public\"\
  ,\n      \"description\": \"Indicates the connection mode and if it is public or private.\"\n    },\n    \"connectorProfileConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Defines the connector-specific profile configuration and credentials.\"\n    }\n  },\n  \"required\": [\n    \"connectorProfileName\",\n    \"connectionMode\",\n    \"connectorProfileConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-update-connector-profile-request-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: UpdateConnectorProfileRequest
---
