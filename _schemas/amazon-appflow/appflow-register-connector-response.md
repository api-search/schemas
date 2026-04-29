---
description: RegisterConnectorResponse schema from Amazon AppFlow API
layout: schema
name: RegisterConnectorResponse
properties_list:
- description: The ARN of the connector being registered.
  name: connectorArn
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-register-connector-response-schema.json
slug: appflow-register-connector-response
source_filename: appflow-register-connector-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-register-connector-response-schema.json\",\n  \"title\": \"RegisterConnectorResponse\",\n  \"description\": \"RegisterConnectorResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorArn\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:appflow:us-east-1:123456789012:connector/MyCustomConnector\",\n      \"description\": \"The ARN of the connector being registered.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-register-connector-response-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: RegisterConnectorResponse
---
