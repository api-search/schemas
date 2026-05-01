---
description: RegisterConnectorRequest schema from Amazon AppFlow API
layout: schema
name: RegisterConnectorRequest
properties_list:
- description: The name of the connector. The name is unique for each ConnectorRegistration in your Amazon Web Services account.
  name: connectorLabel
  type: string
- description: A description about the connector that's being registered.
  name: description
  type: string
- description: The provisioning type of the connector. Currently the only supported value is LAMBDA.
  name: connectorProvisioningType
  type: string
- description: The provisioning type of the connector.
  name: connectorProvisioningConfig
  type: object
- description: Idempotency token.
  name: clientToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-register-connector-request-schema.json
slug: appflow-register-connector-request
source_filename: appflow-register-connector-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-register-connector-request-schema.json\",\n  \"title\": \"RegisterConnectorRequest\",\n  \"description\": \"RegisterConnectorRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorLabel\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"MyCustomConnector\",\n      \"description\": \"The name of the connector. The name is unique for each ConnectorRegistration in your Amazon Web Services account.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"maxLength\": 2048,\n      \"example\": \"My custom connector for proprietary data source\",\n      \"description\": \"A description about the connector that's being registered.\"\n    },\n    \"connectorProvisioningType\": {\n      \"type\": \"string\",\n\
  \      \"enum\": [\n        \"LAMBDA\"\n      ],\n      \"example\": \"LAMBDA\",\n      \"description\": \"The provisioning type of the connector. Currently the only supported value is LAMBDA.\"\n    },\n    \"connectorProvisioningConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"lambda\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"lambdaArn\": {\n              \"type\": \"string\",\n              \"example\": \"arn:aws:lambda:us-east-1:123456789012:function:my-connector-function\",\n              \"description\": \"Lambda ARN of the connector being registered.\"\n            }\n          },\n          \"description\": \"Contains information about the configuration of the lambda which is being registered as the connector.\"\n        }\n      },\n      \"description\": \"The provisioning type of the connector.\"\n    },\n    \"clientToken\": {\n      \"type\": \"string\",\n      \"example\": \"client-token-500123\",\n      \"\
  description\": \"Idempotency token.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-register-connector-request-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: RegisterConnectorRequest
---
