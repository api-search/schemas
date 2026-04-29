---
description: UpdateConnectorRegistrationRequest schema from Amazon AppFlow API
layout: schema
name: UpdateConnectorRegistrationRequest
properties_list:
- description: The name of the connector. The name is unique for each ConnectorRegistration in your Amazon Web Services account.
  name: connectorLabel
  type: string
- description: A description about the update that you're making to the connector.
  name: description
  type: string
- description: The provisioning type of the connector.
  name: connectorProvisioningConfig
  type: object
- description: Idempotency token.
  name: clientToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-update-connector-registration-request-schema.json
slug: appflow-update-connector-registration-request
source_filename: appflow-update-connector-registration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-update-connector-registration-request-schema.json\",\n  \"title\": \"UpdateConnectorRegistrationRequest\",\n  \"description\": \"UpdateConnectorRegistrationRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorLabel\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"MyCustomConnector\",\n      \"description\": \"The name of the connector. The name is unique for each ConnectorRegistration in your Amazon Web Services account.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"maxLength\": 2048,\n      \"example\": \"Updated description for my connector\",\n      \"description\": \"A description about the update that you're making to the connector.\"\n    },\n    \"connectorProvisioningConfig\": {\n\
  \      \"type\": \"object\",\n      \"properties\": {\n        \"lambda\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"lambdaArn\": {\n              \"type\": \"string\",\n              \"example\": \"arn:aws:lambda:us-east-1:123456789012:function:my-connector-function-v2\",\n              \"description\": \"Lambda ARN of the connector being registered.\"\n            }\n          }\n        }\n      },\n      \"description\": \"The provisioning type of the connector.\"\n    },\n    \"clientToken\": {\n      \"type\": \"string\",\n      \"example\": \"client-token-500123\",\n      \"description\": \"Idempotency token.\"\n    }\n  },\n  \"required\": [\n    \"connectorLabel\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-update-connector-registration-request-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: UpdateConnectorRegistrationRequest
---
